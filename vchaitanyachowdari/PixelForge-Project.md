# PixelForge 🎨

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](./package.json)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8.3-blue.svg)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-19.0.0-blue.svg)](https://reactjs.org/)

AI-powered image generation platform with professional tools and user management, built with modern web technologies and production-ready architecture.

## ✨ Features

- 🤖 **AI Image Generation** - Powered by OpenAI and Google Cloud AI Platform
- 👤 **User Authentication** - Secure OAuth integration with Mocha
- 💳 **Wallet Management** - Credit-based system with auto-recharge
- 🎯 **Multiple Generation Types** - Lifestyle, studio, seasonal, e-commerce
- 📱 **Responsive Design** - Mobile-first approach with Tailwind CSS
- ⚡ **Serverless Architecture** - Built on Cloudflare Workers
- 🔒 **Production Ready** - Comprehensive security and monitoring

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm 8+
- Cloudflare account for deployment
- OpenAI API key
- Google Cloud account (optional, for advanced features)

### Installation

```bash
# Clone the repository
git clone https://github.com/your-org/pixelforge.git
cd pixelforge

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env.local
# Edit .env.local with your configuration

# Start development server
npm run dev
```

### Environment Setup

See [Environment Configuration Guide](./docs/ENVIRONMENT.md) for detailed setup instructions.

## 🏗️ Architecture

PixelForge follows **Domain-Driven Design (DDD)** principles with a clean architecture:

```
src/
├── domain/           # Business logic and entities
├── application/      # Use cases and DTOs
├── infrastructure/   # External dependencies
├── presentation/     # API routes and web UI
└── shared/          # Common utilities
```

For complete architecture details, see [Production Transformation Guide](./docs/PRODUCTION_TRANSFORMATION.md).

## 📦 Tech Stack

### Frontend
- **React 19** - UI framework
- **TypeScript** - Type safety
- **Tailwind CSS** - Styling
- **Vite** - Build tool
- **React Router v7** - Navigation

### Backend
- **Hono** - Web framework
- **Cloudflare Workers** - Serverless runtime
- **D1 Database** - SQLite-compatible database
- **Zod** - Schema validation

### AI & External Services
- **OpenAI API** - Image generation
- **Google Cloud AI Platform** - Advanced AI features
- **Mocha Users Service** - Authentication

## 🛠️ Development

### Available Scripts

```bash
# Development
npm run dev                 # Start development server
npm run type-check         # TypeScript checking

# Testing
npm run test               # Run tests
npm run test:coverage      # Coverage report
npm run test:ui           # Test UI

# Code Quality
npm run lint              # ESLint checking
npm run format            # Format with Prettier

# Building
npm run build             # Production build
npm run preview           # Preview build

# Deployment
npm run deploy:staging    # Deploy to staging
npm run deploy:production # Deploy to production
```

### Project Structure

See [Production Transformation Guide](./docs/PRODUCTION_TRANSFORMATION.md) for detailed project structure documentation.

## 🧪 Testing

Comprehensive testing setup with:

- **Unit Tests** - Vitest + Testing Library
- **Integration Tests** - API and component integration
- **E2E Tests** - Full user journey testing
- **Coverage Reports** - Detailed test coverage

```bash
npm run test              # Run all tests
npm run test:coverage     # Generate coverage report
```

## 🚀 Deployment

### Staging

```bash
npm run deploy:staging
```

### Production

```bash
npm run deploy:production
```

For detailed deployment instructions, see [Environment Configuration](./docs/ENVIRONMENT.md).

## 📊 Monitoring & Performance

- **Error Tracking** - Sentry integration ready
- **Performance Monitoring** - Web Vitals tracking
- **Analytics** - User behavior insights
- **Health Checks** - Application health monitoring

## 🔒 Security

- **Environment Variables** - Secure secret management
- **Input Validation** - Zod schema validation
- **Authentication** - OAuth2 integration
- **Rate Limiting** - API abuse prevention
- **CORS Configuration** - Cross-origin security

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow TypeScript best practices
- Write comprehensive tests
- Follow the established architecture patterns
- Update documentation for new features

## 📄 Documentation

- [Environment Configuration](./docs/ENVIRONMENT.md)
- [Production Transformation Guide](./docs/PRODUCTION_TRANSFORMATION.md)
- [API Documentation](./docs/API.md) (Coming soon)
- [Deployment Guide](./docs/DEPLOYMENT.md) (Coming soon)

## 🐛 Support

Join our [Discord community](https://discord.gg/shDEGBSe2d) for:

- Technical support
- Feature discussions
- Community feedback
- Development updates

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built with [Mocha Framework](https://getmocha.com)
- Powered by [Cloudflare Workers](https://workers.cloudflare.com/)
- AI capabilities by [OpenAI](https://openai.com/) and [Google Cloud](https://cloud.google.com/)

---

**PixelForge** - Transform your ideas into stunning visuals with the power of AI. 🚀
