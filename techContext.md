# Technical Context for MCP Server

## Development Environment
- Python 3.11+
- Poetry for dependency management
- Hatchling as build backend
- VSCode as primary development environment

## Dependencies
- mcp (>=1.1.0)
- python-dotenv (>=1.0.1)
- requests (>=2.32.3)

## Technical Requirements
1. Asynchronous Server Implementation
   - Uses asyncio for concurrent operations
   - Stdio-based transport mechanism
   - Non-blocking tool execution

2. Configuration Management
   - Environment variable-based configuration
   - Support for multiple vault configurations
   - Secure credential handling

3. Error Handling
   - Comprehensive logging
   - Detailed error tracking
   - Graceful error recovery

## Development Tools
- pyright for type checking
- Logging configured to stderr
- Supports multiple implementation strategies

## Compatibility Considerations
- Flexible LLM interface support
- OpenRouter model integration
- Local model support via Ollama
- Claude model compatibility

## Performance Expectations
- Low-latency tool execution
- Minimal resource overhead
- Scalable multi-vault support
