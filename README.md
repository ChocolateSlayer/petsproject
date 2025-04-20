# Pet Service

A modern Go-based service for connecting cat owners with cat sitters, featuring scheduling, chat, and video call capabilities.

## Features

- 🐱 Cat owner and sitter profiles
- 📅 Scheduling system
- 💬 Real-time chat
- 📹 Video calls
- 📊 Metrics and monitoring
- 🚀 Kubernetes deployment

## Tech Stack

- Go 1.24
- Gin Web Framework
- gRPC
- WebSocket
- WebRTC
- PostgreSQL
- Redis
- Prometheus
- Jaeger
- Docker
- Kubernetes

## Project Structure

```
.
├── cmd/                    # Application entrypoints
│   └── server/            # Main server application
├── internal/              # Private application code
│   ├── domain/           # Business logic and entities
│   ├── repository/       # Data access layer
│   ├── service/          # Business logic implementation
│   ├── delivery/         # HTTP/gRPC handlers
│   └── infrastructure/   # External services integration
├── pkg/                  # Public libraries
├── api/                  # API definitions (proto files)
├── deployments/          # Kubernetes manifests
├── scripts/              # Build and deployment scripts
└── test/                 # Integration tests
```

## Getting Started

### Prerequisites

- Go 1.21 or higher
- Docker
- Kubernetes cluster (local or remote)
- Make

### Development Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   go mod download
   ```
3. Run the service:
   ```bash
   make run
   ```

### Building

```bash
make build
```

### Testing

```bash
make test
```

## API Documentation

API documentation will be available at `/swagger/index.html` when running the service.

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 