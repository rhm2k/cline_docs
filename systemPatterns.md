# MCP Server System Patterns

## Architecture
- MCP servers act as intermediaries between LLMs and external tools/resources
- Provide a standardized interface for tool and resource access
- Support multiple vault/server configurations
- Handle both local and remote resource access

## Key Components
1. Server Initialization
   - Load configuration from environment variables
   - Set up tool handlers with proper error boundaries
   - Initialize secure transport layer
   - Configure SSL certificate handling

2. Tool Management
   - Dynamic tool registration with validation
   - Tool description generation following MCP protocol
   - Strict argument validation and type checking
   - Comprehensive error handling with proper logging

3. Resource Handling
   - Multi-vault configuration with independent settings
   - Resource listing with proper error handling
   - Secure access control with API key validation
   - SSL certificate management for secure connections

## Communication Patterns
1. Transport Layer
   - Custom StdioTransport implementation
   - Asynchronous read/write operations
   - Proper stream handling and cleanup
   - Error recovery mechanisms

2. Protocol Implementation
   - Strict JSON message format validation
   - Standardized request/response structure
   - Proper error response formatting
   - Message type validation

3. Connection Management
   - Graceful connection handling
   - Proper resource cleanup
   - Connection recovery mechanisms
   - Event loop management

## Security Considerations
1. SSL Management
   - Custom certificate handling for localhost
   - Proper SSL verification for remote connections
   - Certificate authority store management
   - SSL error handling and logging

2. Access Control
   - Isolated vault configurations
   - Secure API key management
   - Transport-level encryption
   - Minimal privilege access

3. Error Handling
   - Secure error message formatting
   - No sensitive data in error responses
   - Proper logging of security events
   - Rate limiting and timeout handling
