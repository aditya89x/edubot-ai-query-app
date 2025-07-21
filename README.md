# EduBot - AI-Powered Student Query App

A comprehensive AI-powered platform for college admissions guidance, featuring ChatGPT-like interactions, verified alumni networking, and social features for students.

## Features

### 🤖 AI Chat Assistant
- Real-time college admission guidance
- Powered by OpenRouter API with GPT-4o
- Specialized prompts for educational guidance
- Quick question suggestions

### 👥 Alumni Network
- Verified alumni from top institutions (IIT, NIT, IIM, MIT, Harvard)
- LinkedIn verification system
- Direct messaging and mentorship
- Search by institution, major, and expertise

### 📱 Social Features
- Student networking and interactions
- Post sharing with likes and comments
- Follow system for users
- Real-time messaging

### 🔐 Authentication
- Complete login/signup system
- Role-based access (Student, Alumni, Counselor)
- Secure user management

## Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: Tailwind CSS, Shadcn UI
- **AI Integration**: OpenRouter API (GPT-4o)
- **Authentication**: Custom auth system
- **Deployment**: Vercel-ready

## Getting Started

### Prerequisites
- Node.js 18+ 
- npm or yarn
- OpenRouter API key

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd edubot-app
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env.local` file in the root directory:
```env
OPENROUTER_API_KEY=your_openrouter_api_key_here
NEXTAUTH_SECRET=your_nextauth_secret_here
NEXTAUTH_URL=http://localhost:3000
```

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## API Key Setup

1. Visit [OpenRouter](https://openrouter.ai/keys)
2. Create a free account
3. Generate an API key
4. Add it to your `.env.local` file

## Project Structure

```
src/
├── app/
│   ├── api/chat/          # AI chat API endpoint
│   ├── auth/              # Authentication pages
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Home page
├── components/
│   ├── ui/                # Shadcn UI components
│   ├── alumni-directory.tsx
│   ├── chat-interface.tsx
│   ├── social-feed.tsx
│   └── auth-provider.tsx
├── types/
│   ├── chat.ts            # Chat-related types
│   └── user.ts            # User and social types
└── lib/
    └── utils.ts           # Utility functions
```

## Features Overview

### AI Chat System
- Specialized system prompt for college guidance
- Real-time responses via OpenRouter API
- Context-aware conversations
- Quick question templates

### Alumni Directory
- Verified profiles with LinkedIn integration
- Search and filter functionality
- Mentorship availability indicators
- Direct messaging capabilities

### Social Platform
- Post creation and sharing
- Like and comment system
- User following/followers
- Real-time interactions

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy automatically

### Manual Deployment

```bash
npm run build
npm start
```

## Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `OPENROUTER_API_KEY` | OpenRouter API key for AI chat | Yes |
| `NEXTAUTH_SECRET` | Secret for authentication | Yes |
| `NEXTAUTH_URL` | Base URL for the application | Yes |

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

For support and questions:
- Create an issue in the repository
- Contact the development team

## Acknowledgments

- OpenRouter for AI API services
- Shadcn for UI components
- Vercel for hosting platform
- Next.js team for the framework
