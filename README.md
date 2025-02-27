# Perplexity Deep Research MCP
[![smithery badge](https://smithery.ai/badge/@arjunkmrm/perplexity-deep-research)](https://smithery.ai/server/@arjunkmrm/perplexity-deep-research)

A Model Context Protocol (MCP) server for Perplexity AI API with web search capabilities. This server allows AI assistants to perform web searches using Perplexity's chat completions API with the sonar-deep-research model.

## Features

- Provides a `deep_research` tool for AI assistants to perform web searches
- Uses Perplexity's chat completions API with the sonar-deep-research model

## Tool: deep_research

The server provides a `deep_research` tool with the following input parameters:

- `query` (required): The search query to perform
- `search_recency_filter` (optional): Filter search results by recency (options: month, week, day, hour)

## Configuration

### Environment Variables

- `PERPLEXITY_API_KEY`: Your Perplexity API key (required)

## Response Format

The response from the `deep_research` tool includes:

- Content of search results
- Citations for the information

## Installing via Smithery

To install perplexity-deep-research for Claude Desktop automatically via [Smithery](https://smithery.ai/server/@arjunkmrm/perplexity-deep-research):

```bash
npx -y @smithery/cli install @arjunkmrm/perplexity-deep-research --client claude
```

## License

MIT 
