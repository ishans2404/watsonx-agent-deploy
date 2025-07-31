# WatsonX Agent Deploy

Simple tool to deploy multiple AI agents to IBM WatsonX.ai

## Installation

```bash
pip install watsonx-agent-deploy
```

## Quick Start

1. Create your agents using WatsonX template:
   ```bash
   watsonx-ai template new "base/langgraph-react-agent" my-agent
   ```

2. Create a `.env` file:
   ```
   WATSONX_APIKEY=your_api_key_here
   WATSONX_URL=https://your-watsonx-url.com
   SPACE_ID=your_space_id
   ```

3. Deploy all agents:
   ```bash
   watsonx-deploy
   ```

## Usage

```bash
# Deploy from current directory
watsonx-deploy

# Deploy with custom .env file
watsonx-deploy --env-file /path/to/.env

# Deploy from specific directory
watsonx-deploy --config-dir /path/to/agents

# Verbose output
watsonx-deploy --verbose
```

## Requirements

- Python 3.8+
- IBM WatsonX.ai CLI
- Agent folders must end with 'agent'
- Each agent folder must contain config.toml

## License

MIT
