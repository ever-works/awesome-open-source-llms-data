## Overview

Firecrawl is a data collection platform built for AI agents. What started as a web scraping API has grown into a full platform handling the hardest part of agent development: getting structured data from the web. Users describe what they want in plain text, optionally pass a Pydantic schema, and the agent searches, navigates, and returns structured results.

## Agent Models

- **spark-1-mini** (default): 60% cheaper, suited for straightforward extractions
- **spark-1-pro**: For complex multi-domain research where accuracy matters most

Both models work without requiring URLs, though URLs can be provided to focus the search.

## Additional Features

- **Browser Sandbox**: Secure, managed browser environment with Playwright pre-installed; execute Python, JavaScript, or bash commands remotely
- **Scrape/Crawl/Batch Scrape**: Endpoints for bulk data collection
- **Map Endpoint**: Generates URL lists from entire sites
- **LLMs.txt API**: Converts websites to clean text for LLMs
- **CLI**: Terminal-based workflows

## Integration

All endpoints can be plugged into any agent framework (LangGraph, AutoGen, CrewAI, etc.) as custom tools, extending agents with reliable web interaction capabilities.

## Best For

Teams building agents that need reliable access to structured web data without writing and maintaining scraping scripts.