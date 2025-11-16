# Welcome to Your Miaoda Project
Miaoda Application Link URL
    URL:https://medo.dev/projects/app-7la5aw4xicch

# Smart Study Companion

An AI-powered personal study assistant that helps students track their studies, analyze performance, understand important topics, and improve learning efficiency through intelligent features.

## 🌟 Features

### Core Features
- **Smart Study Tracker**: Track study sessions with timer, subject tagging, difficulty levels, and importance ratings
- **AI Study Analysis**: Upload documents and get AI-powered insights, summaries, MCQs, and revision notes
- **Analytics Dashboard**: View your study progress, XP points, level, streak, and recent activities
- **Gamification**: Earn XP, level up, unlock achievements, and maintain study streaks
- **Profile Management**: Track your progress and manage your account
- **Dark Mode**: Beautiful light and dark themes with smooth transitions

### Coming Soon
- Advanced analytics with charts and visualizations
- Flashcard system with spaced repetition
- Study planner with AI-generated schedules
- Voice assistant integration
- Smart notifications
- Heatmap calendar visualization

## 🎨 Design

- **Color Scheme**: Calming blues and greens for focus, energetic orange/yellow for motivation
- **UI Components**: Built with shadcn/ui for consistent, modern design
- **Responsive**: Works seamlessly on desktop and mobile devices
- **Animations**: Smooth transitions and elegant interactions

## 🛠️ Tech Stack

- **Frontend**: React 18 + TypeScript + Vite
- **UI Library**: shadcn/ui + Tailwind CSS
- **Backend**: Supabase (Database, Auth, Storage)
- **AI Services**:
  - Gemini 2.5 Flash for document analysis and question generation
  - OCR.space for handwritten note processing
  - Text-to-Speech API for voice features (ready for integration)
- **Authentication**: Google SSO via Supabase Auth

## 📋 Prerequisites

- Node.js ≥ 20
- npm ≥ 10
- Supabase account
- API keys for AI services (Gemini, OCR.space, TTS)

## 🚀 Getting Started

### 1. Environment Setup

Create a `.env` file in the root directory with the following variables:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
VITE_GEMINI_API_KEY=your_gemini_api_key
VITE_OCR_API_KEY=your_ocr_space_api_key
VITE_TTS_API_KEY=your_tts_api_key
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Database Setup

The database schema is already configured in `supabase/migrations/`. The following tables are created:
- `profiles` - User profiles with XP, level, and streak tracking
- `subjects` - Study subjects
- `study_sessions` - Study session records
- `documents` - Uploaded documents and notes
- `flashcards` - Flashcard system
- `quizzes` - Quiz questions and answers
- `quiz_attempts` - Quiz attempt records
- `study_plans` - Study planning and scheduling
- `achievements` - Gamification achievements
- `notifications` - User notifications

### 4. Run Development Server

```bash
npm run dev -- --host 127.0.0.1
```

Or if the above fails:

```bash
npx vite --host 127.0.0.1
```

### 5. Build for Production

```bash
npm run build
```

## 📁 Project Structure

```
├── src/
│   ├── components/
│   │   ├── auth/          # Authentication components
│   │   ├── common/        # Shared components (Header, ThemeToggle)
│   │   └── ui/            # shadcn/ui components
│   ├── contexts/          # React contexts (AuthContext)
│   ├── db/
│   │   ├── api.ts         # Database API functions
│   │   └── supabase.ts    # Supabase client
│   ├── pages/             # Page components
│   │   ├── Dashboard.tsx
│   │   ├── StudyTimer.tsx
│   │   ├── AIAnalysis.tsx
│   │   ├── Analytics.tsx
│   │   ├── Flashcards.tsx
│   │   ├── StudyPlanner.tsx
│   │   ├── Profile.tsx
│   │   ├── Login.tsx
│   │   └── Signup.tsx
│   ├── services/          # External service integrations
│   │   └── aiService.ts   # AI service (Gemini, OCR, TTS)
│   ├── types/             # TypeScript type definitions
│   ├── App.tsx            # Main app component
│   ├── routes.tsx         # Route configuration
│   └── index.css          # Global styles and design tokens
├── supabase/
│   └── migrations/        # Database migrations
├── public/                # Static assets
└── README.md
```

## 🔐 Authentication

The app uses Supabase Authentication with Google SSO. Users can:
- Sign up with email/password
- Sign in with Google
- Manage their profile
- Track their progress and achievements

## 🎮 Gamification System

- **XP Points**: Earn points by studying and completing activities
- **Levels**: Progress through levels as you earn XP (1000 XP per level)
- **Streaks**: Maintain daily study streaks
- **Achievements**: Unlock achievements for milestones

## 🤖 AI Features

### Document Analysis
- Upload PDFs, images, or text files
- Extract text using OCR for handwritten notes
- Generate summaries, important topics, MCQs, and revision notes
- Powered by Gemini 2.5 Flash

### Coming Soon
- Weakness detection and personalized recommendations
- AI-generated study schedules
- Voice assistant for hands-free interaction
- Exam score predictions

## 📱 Responsive Design

The app is fully responsive and works on:
- Desktop (1920x1080, 1366x768, 1440x900)
- Laptop (1280x720, 1536x864)
- Mobile (375x667, 414x896, 430x932)

## 🎨 Customization

### Theme Colors
The app uses a semantic color system defined in `src/index.css`:
- Primary: Calming blue (#3B82F6)
- Secondary: Refreshing green (#10B981)
- Accent: Energetic orange (#F59E0B)
- Success, Warning, Destructive colors for different states

### Dark Mode
Toggle between light and dark themes using the theme switcher in the header.

## 🧪 Development

### Linting
```bash
npm run lint
```

### Type Checking
```bash
npm run type-check
```

## 📝 License

This project is part of the Miaoda platform.

## 🤝 Contributing

This is a generated project from Miaoda. For contributions and support, please refer to the Miaoda documentation.

## 📚 Learn More

- [Miaoda Documentation](https://intl.cloud.baidu.com/en/doc/MIAODA/)
- [Supabase Documentation](https://supabase.com/docs)
- [shadcn/ui Documentation](https://ui.shadcn.com/)
- [React Documentation](https://react.dev/)

## 🎯 Roadmap

See [TODO.md](./TODO.md) for detailed implementation status and future plans.

---

Built with ❤️ using Miaoda
