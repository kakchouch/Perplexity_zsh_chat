# Perplexity Chat Zsh Script

## Description

A lightweight command-line interface for Perplexity AI built in pure Zsh, allowing you to interact with the Perplexity API directly from your terminal.

## Prerequisites

- Zsh shell
- `curl` command-line tool
- `jq` JSON processor
- A valid Perplexity API key

## Installation

1. Clone or download the script to your local machine
2. Make the script executable:
   ```bash
   chmod +x perplexity.sh
   ```
3. Set your API key as an environment variable:
   ```bash
   export PERPLEXITY_API_KEY="your_api_key_here"
   ```

## Configuration

Edit the script to customize:
- **Model selection**: Change the `model` parameter (e.g., `sonar-pro`, `pplx-7b-online`)
- **System prompt**: Modify the `system` message for different assistant behaviors
- **Request parameters**: Adjust temperature, max tokens, and other API options

## Usage

Run the script with your query as an argument:

```bash
./perplexity.sh "Your question here"
```

Or in interactive mode:

```bash
./perplexity.sh
```

## API Endpoint

The script communicates with:[1]
```
https://api.perplexity.ai/chat/completions
```

## Authentication

Authentication uses Bearer token validation with your API key passed in the request headers[2].

## Features

- Real-time AI responses from Perplexity
- Support for streaming and non-streaming responses
- Customizable system prompts and model parameters
- Simple command-line interface

## Troubleshooting

- **"API key not found"**: Ensure `PERPLEXITY_API_KEY` environment variable is set
- **JSON parsing errors**: Verify `jq` is installed: `which jq`
- **Connection timeouts**: Check internet connection and API endpoint availability

## License

MIT License

## Support

For issues or questions, refer to the Perplexity API documentation or GitHub repository.
