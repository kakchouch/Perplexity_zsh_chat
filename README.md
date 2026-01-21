# Perplexity Chat Zsh Script

## Description

A lightweight command-line interactive chat for Perplexity AI built in pure Zsh, allowing you to interact with the Perplexity API directly from your terminal.

## Prerequisites

- Zsh shell
- `curl` command-line tool
- `jq` JSON processor
- A valid Perplexity API key

## Installation

1. Clone or download the script to your local machine
2. Make the script executable:
   ```bash
   chmod +x perpchat
   ```
3. Set your API key as an environment variable:
   ```bash
   export PERPLEXITY_API_KEY="your_api_key_here"
   ```
Consider entering the previous command in your .zshrc for ease of use.

## Configuration

Edit the script to customize:
- **Model selection**: Change the `model` parameter (e.g., `sonar-pro`, `pplx-7b-online`)
The following feature are not yet implemented :
- **System prompt**: Modify the `system` message for different assistant behaviors
- **Request parameters**: Adjust temperature, max tokens, and other API options

## Usage

Run the script with your query as an argument:

```bash
./perpchat
```
Consider adding the directory in your $PATH.
You can leave the interactive chat by entering 'exit' or hitting CTRL+C.

Chat is saved in $HOME/perplexity_chats upon leaving the chat.

## API Endpoint

The script communicates with:[1]
```
https://api.perplexity.ai/chat/completions
```
The 'Threads' and 'Spaces' APIs are not public (according to my current knowledge). Therefore, assume all chats conducting through this script are agnostic of your perplexity history.

## Authentication

Authentication uses Bearer token validation with your API key passed in the request headers.

## Features

- Real-time AI responses from Perplexity
- Customizable model parameters
- Simple command-line interface

## Troubleshooting

- **"API key not found"**: Ensure `PERPLEXITY_API_KEY` environment variable is set
- **JSON parsing errors**: Verify `jq` is installed: `which jq`
- **Connection timeouts**: Check internet connection and API endpoint availability

## License

MIT License

## Support

For issues or questions, refer to the Perplexity API documentation or GitHub repository.
