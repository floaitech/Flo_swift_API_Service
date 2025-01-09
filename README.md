# Flo AI API Services

A collection of high-performance Swift API services for AI image generation and natural language processing.

## Services

### 1. ChatGPT API
High-throughput OpenAI GPT integration with streaming support and context management.
- Streaming responses
- Context management
- Rate limiting
- Error handling

### 2. Replicate API
Production-ready Replicate.com API integration for various AI models.
- Model version management
- Prediction pipeline
- Progress tracking
- Result caching

### 3. ComfyUI AWS API
Enterprise-grade ComfyUI integration with AWS infrastructure.
- AWS Lambda integration
- S3 storage
- CloudFront CDN
- DynamoDB state management

### 4. Fooocus API
Specialized API service for the Fooocus image generation model.
- Custom workflows
- Advanced parameters
- Result optimization
- Quality presets

## Architecture

- **Thread Safety**: All services are thread-safe and designed for concurrent access
- **Memory Management**: Efficient resource handling with automatic cleanup
- **Error Handling**: Comprehensive error types and recovery strategies
- **Monitoring**: Built-in performance metrics and logging

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/yourusername/flo-api-services.git
cd flo-api-services
```

2. Copy and configure environment:
```bash
cp Config.xcconfig.example Config.xcconfig
# Edit Config.xcconfig with your API keys and credentials
```

3. Install dependencies:
```bash
# If using SPM
swift package resolve
```

## Configuration

Each service requires specific API keys and configuration:

- **ChatGPT**: OpenAI API key
- **Replicate**: Replicate API token
- **ComfyUI**: AWS credentials and region
- **Fooocus**: Model-specific configuration

See `Config.xcconfig.example` for all required variables.

## Usage Examples

### ChatGPT Service
```swift
let service = ChatGPTService()
service.sendMessage("Hello, world!") { result in
    switch result {
    case .success(let response):
        print(response.content)
    case .failure(let error):
        print(error)
    }
}
```

### Replicate Service
```swift
let service = ReplicateService()
service.generateImage(prompt: "sunset beach") { result in
    switch result {
    case .success(let image):
        // Handle image
    case .failure(let error):
        // Handle error
    }
}
```

## Security

- All API keys stored securely
- AWS IAM best practices
- Request signing
- Input validation

## Performance

- Concurrent request handling
- Response streaming
- Result caching
- Resource pooling

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License - see LICENSE file

## Support

For support, please open an issue in the GitHub repository. 