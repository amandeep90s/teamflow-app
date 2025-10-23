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
- `bun format` - Format code with Prettier (includes Tailwind class sorting)
- `bun format:check` - Check code formatting
- `bun sort-imports` - Sort imports according to priority

## 🔧 Code Standards

### Import Order Priority

The project uses ESLint to automatically sort imports in the following order:

1. **React & Next.js** - `react`, `react-dom`, `next/*`
2. **External libraries** - Third-party packages
3. **UI libraries** - `@radix-ui/*`, `lucide-react`
4. **Internal modules** - `@/*` (with path mapping)
5. **Relative imports** - `./`, `../`
6. **CSS imports** - `.css` files

Example:

```tsx
import React from 'react';
import { NextPage } from 'next';

import { Button } from '@radix-ui/react-button';
import { ChevronDown } from 'lucide-react';

import { MyComponent } from '@/components/MyComponent';
import { utils } from '@/lib/utils';

import { LocalComponent } from './LocalComponent';

import './styles.css';
```

### Tailwind CSS Class Sorting

Prettier automatically sorts Tailwind CSS classes using the official plugin. Classes are organized by:

1. **Layout** - `container`, `box-sizing`, `display`, `position`
2. **Spacing** - `margin`, `padding`
3. **Sizing** - `width`, `height`, `min/max`
4. **Typography** - `font-*`, `text-*`, `line-height`
5. **Backgrounds** - `bg-*`
6. **Borders** - `border-*`, `rounded-*`
7. **Effects** - `shadow-*`, `opacity`, `transform`
8. **Interactivity** - `hover:`, `focus:`, `active:`
9. **Responsive** - `sm:`, `md:`, `lg:`, `xl:`, `2xl:`

Example:

```tsx
// Before
<div className="hover:bg-blue-500 text-white p-4 bg-blue-400 rounded-lg shadow-md">

// After (automatically sorted)
<div className="rounded-lg bg-blue-400 p-4 text-white shadow-md hover:bg-blue-500">
```

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
