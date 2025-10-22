# TeamFlow App

A modern, real-time collaboration platform built with cutting-edge technologies. TeamFlow provides a seamless experience for team communication with advanced features like AI-powered thread summarization, real-time messaging, and comprehensive security.

## ✨ Features

### 🚀 Core Technology Stack

- 🌐 **Next.js 15** - Latest React framework with app directory
- 🎨 **Tailwind CSS & Shadcn UI** - Beautiful, responsive design system
- 🧮 **Neon Postgres** - Serverless PostgreSQL database
- 💾 **Prisma ORM** - Type-safe database access
- 🚀 **Vercel** - Optimized deployment platform

### 🔐 Authentication & Security

- 🔒 **Kinde Authentication** - OAuth & Magic Links support
- 🛡️ **Arcjet Security** - Protection against XSS, SQL injection, and other attacks
- 🚫 **Rate Limiting** - Intelligent request throttling
- 💂 **Self-serve Customer Portal** - User account management

### 💬 Communication Features

- 👨‍🚀 **Thread Support** - Organized conversations
- 🚀 **AI Thread Summarization & Composer** - Smart content generation
- 🏎️ **Real-time Messaging** - Powered by Cloudflare Durable Objects
- 🫣 **Emoji Reactions** - Express yourself with emojis
- 👾 **Custom Rich Text Editor** - Advanced message formatting
- 🖊️ **Edit Messages** - Modify sent messages
- 📜 **Reverse Infinite Scroll** - Smooth message history navigation

### 🏢 Organization & Collaboration

- 🧠 **Organizations** - Multi-tenant support
- 🦾 **Channels** - Organize conversations by topic
- 👥 **Invite Members** - Easy team onboarding
- ✅ **Real-time Presence** - See who's online
- 🖼️ **Image Uploads** - Secure file sharing with presigned URLs

### 💰 Business Features

- 💵 **Billing System** - Monthly subscription tiers
- 📊 **Usage Analytics** - Track platform metrics

### 🛠️ Architecture & Performance

- ✅ **Performance-Optimized** - Fast loading and smooth interactions
- ✅ **Clean, Secure Codebase** - Maintainable and scalable architecture
- ✅ **Data Access Layer & DTO** - Structured data handling
- 🔧 **ESLint & Prettier** - Code quality and formatting

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ or Bun
- PostgreSQL database (Neon recommended)

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd teamflow-app
   ```

2. **Install dependencies**

   ```bash
   bun install
   # or
   npm install
   ```

3. **Set up environment variables**

   ```bash
   cp .env.example .env.local
   ```

   Fill in your environment variables for:
   - Database connection (Neon)
   - Kinde authentication
   - Arcjet security keys
   - Cloudflare Durable Objects
   - Other service credentials

4. **Run database migrations**

   ```bash
   bun run db:migrate
   # or
   npm run db:migrate
   ```

5. **Start the development server**

   ```bash
   bun dev
   # or
   npm run dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 📜 Available Scripts

- `bun dev` - Start development server
- `bun build` - Build for production
- `bun start` - Start production server
- `bun lint` - Run ESLint
- `bun lint:fix` - Fix ESLint issues
- `bun format` - Format code with Prettier
- `bun format:check` - Check code formatting

## 🏗️ Project Structure

```
teamflow-app/
├── app/                    # Next.js app directory
├── components/            # Reusable UI components
├── lib/                   # Utility functions and configurations
├── prisma/               # Database schema and migrations
├── public/               # Static assets
└── types/                # TypeScript type definitions
```

## 🚀 Deployment

This application is optimized for deployment on Vercel:

1. Connect your repository to Vercel
2. Configure environment variables
3. Deploy automatically on every push to main

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

Built with modern web technologies and best practices for scalable team collaboration.
