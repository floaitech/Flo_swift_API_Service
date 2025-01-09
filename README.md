# Flo AI API Services

Swift implementation of AI services for image generation and text processing.

## Services

### ChatGPT API
- Streaming responses
- Context management
- Rate limiting
- Error handling

### Replicate API
- Model version management
- Prediction pipeline
- Progress tracking
- Result caching

### ComfyUI AWS API
- AWS Lambda integration
- S3 storage
- CloudFront CDN
- DynamoDB state management

### Fooocus API
- Custom workflows
- Advanced parameters
- Result optimization

## Setup

1. Clone and configure:
```bash
git clone https://github.com/floaitech/Flo_swift_API_Service.git
cd Flo_swift_API_Service
cp Config.xcconfig.example Config.xcconfig
# Add your API keys to Config.xcconfig
```

## Required Keys

| Service | Key | Purpose |
|---------|-----|---------|
| OpenAI | `OPENAI_API_KEY` | ChatGPT access |
| Replicate | `REPLICATE_API_KEY` | Model access |
| AWS | `AWS_ACCESS_KEY` | AWS services |
| AWS | `AWS_SECRET_KEY` | AWS auth |

## Usage

See individual service README files:
- [ChatGPT API](ChatGPT%20API/README.md)
- [Replicate API](Replicate%20API/README.md)
- [ComfyUI AWS](ComfyUI%20AWS%20Fooocus%20API%20(Current)/README.md)
- [Fooocus API](Replicate%20Fooocus%20API/README.md)

## License

MIT License - see [LICENSE](LICENSE) 