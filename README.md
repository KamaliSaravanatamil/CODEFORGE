# CodeForge AI 🚀

A voice-first, multi-agent orchestration platform that democratizes coding education for Indian language speakers.

## Overview

CodeForge AI transforms user ideas into production-ready applications through intelligent AI mentorship, providing hands-on learning experiences in Hindi and Tamil. The platform combines natural language understanding with specialized AI agents that guide users through project planning, code generation, learning, and deployment.

## Key Features

- **Voice-First Interface**: Code naturally in Hindi or Tamil using voice commands
- **Multi-Agent System**: Specialized AI agents for planning, coding, and tutoring
- **Real-Time Collaboration**: Pair program with teammates in real-time
- **Stage-Wise Learning**: Progressive milestones adapted to your skill level
- **Instant Deployment**: One-click deployment to Vercel or AWS Lambda
- **Hackathon Mode**: Generate complete project scaffolds in under 60 seconds
- **Affordable Access**: ₹99/month subscription with 7-day free trial

## Architecture

CodeForge AI follows a microservices architecture with:

- **Frontend**: React 18 + TypeScript + Monaco Editor
- **Backend**: Node.js + Express + LangChain.js
- **Database**: PostgreSQL + Redis
- **AI Agents**: Supervisor, Planner, Coder, and Tutor agents
- **Real-Time**: Socket.IO for collaboration
- **Deployment**: Vercel and AWS Lambda integration

## Getting Started

### Prerequisites

- Node.js 18+ and npm/yarn
- PostgreSQL 14+
- Redis 6+
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/KamaliSaravanatamil/CODEFORGE.git
cd CODEFORGE

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Run database migrations
npm run migrate

# Start development server
npm run dev
```

### Environment Variables

Create a `.env` file with the following:

```env
# Database
DATABASE_URL=postgresql://user:password@localhost:5432/codeforge
REDIS_URL=redis://localhost:6379

# AI/LLM
OPENAI_API_KEY=your_openai_key
ANTHROPIC_API_KEY=your_anthropic_key

# Authentication
JWT_SECRET=your_jwt_secret
SESSION_SECRET=your_session_secret

# Deployment
VERCEL_TOKEN=your_vercel_token
AWS_ACCESS_KEY_ID=your_aws_key
AWS_SECRET_ACCESS_KEY=your_aws_secret

# Payment
RAZORPAY_KEY_ID=your_razorpay_key
RAZORPAY_KEY_SECRET=your_razorpay_secret
```

## Project Structure

```
CODEFORGE/
├── src/
│   ├── components/       # React components
│   ├── services/         # API and business logic
│   ├── agents/           # AI agent implementations
│   ├── state/            # State management
│   └── hooks/            # Custom React hooks
├── server/
│   ├── api/              # API routes
│   ├── agents/           # Backend agent logic
│   ├── services/         # Backend services
│   └── db/               # Database models and migrations
├── design.md             # Detailed design document
├── requirements.md       # Requirements specification
└── tasks.md              # Implementation tasks
```

## Usage

### Voice Commands (Hindi/Tamil)

```
"नया प्रोजेक्ट बनाओ" (Create new project)
"कोड जेनरेट करो" (Generate code)
"यह कैसे काम करता है?" (How does this work?)
"डिप्लॉय करो" (Deploy)
```

### Code Generation

```javascript
// Request via voice or text
"Create a REST API for user authentication with JWT"

// CodeForge generates production-ready code with:
// - Proper error handling
// - Security best practices
// - Inline documentation
// - Test cases
```

### Collaboration

```bash
# Share your project
npm run share-session

# Join a session
npm run join-session <session-id>
```

## Development

### Running Tests

```bash
# Run all tests
npm test

# Run with coverage
npm run test:coverage

# Run specific test suite
npm test -- agents
```

### Building for Production

```bash
# Build frontend and backend
npm run build

# Start production server
npm start
```

## Deployment

### Deploy to Vercel

```bash
npm run deploy:vercel
```

### Deploy to AWS Lambda

```bash
npm run deploy:aws
```

## Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Roadmap

- [ ] Support for more Indian languages (Bengali, Telugu, Marathi)
- [ ] Mobile app for iOS and Android
- [ ] Advanced debugging tools with AI assistance
- [ ] Integration with popular IDEs (VS Code, IntelliJ)
- [ ] Community marketplace for project templates
- [ ] Enterprise features for teams and organizations

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

- **Documentation**: [docs.codeforge.ai](https://docs.codeforge.ai)
- **Discord Community**: [discord.gg/codeforge](https://discord.gg/codeforge)
- **Email**: support@codeforge.ai
- **Twitter**: [@CodeForgeAI](https://twitter.com/CodeForgeAI)

## Acknowledgments

- Built with ❤️ for Indian developers
- Powered by OpenAI GPT-4 and Anthropic Claude
- Special thanks to the open-source community

---

**Made with 🇮🇳 in India**
