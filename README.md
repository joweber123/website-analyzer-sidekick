This program will look through websites and try to find certain predefined keywords. You'll need to put in a CloudFlare workers key and an OpenAI API key for this to work. It will save those keys to your local browser and gives you the ability to purge them from storage as well.

## Features

- **Multi-Domain Support**: Analyze up to 30 websites concurrently
- **Intelligent Content Extraction**: AI-powered page selection for relevant content
- **Service Detection**: Automatically detects e-commerce, WordPress, WooCommerce, web design services, and more
- **Team & Contact Extraction**: Finds team members, phone numbers, and email addresses
- **Export Results**: Download comprehensive analysis results as JSON
- **Cost Tracking**: Real-time tracking of API usage and costs

## Usage

### Single Domain Analysis
Enter one domain in the input field:
```
example.com
```

### Multi-Domain Analysis
Enter multiple domains (one per line) - up to 30 domains:
```
example.com
another-site.com
agency-website.com
```

The analyzer will process all domains concurrently (3 at a time) for optimal performance.

### URL Parameters

You can automatically search for sites once your API keys are configured by adding a query to the URL.

**Single domain:**
```
https://joweber123.github.io/website-analyzer-sidekick/?domain=agency-website.com
```

**Multiple domains (comma-separated):**
```
https://joweber123.github.io/website-analyzer-sidekick/?domains=example.com,another-site.com,agency-website.com
```

## Requirements

- Cloudflare Worker URL (CORS proxy)
- OpenAI API Key (GPT-5-nano or GPT-4o-mini)
