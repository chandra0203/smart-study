# Smart Study Companion - Setup Guide

## 🚀 Quick Start

Your Smart Study Companion app is ready to use! Follow these steps to get started.

## ✅ What's Already Done

The following has been set up for you:
- ✅ Complete database schema with 10 tables
- ✅ Supabase authentication with Google SSO
- ✅ Document storage bucket
- ✅ All core pages and components
- ✅ Beautiful UI with dark mode support
- ✅ AI service integration (ready for API keys)

## 🔑 Required: API Keys Setup

You need to obtain and configure the following API keys in your `.env` file:

### 1. Gemini API Key (Required for AI Analysis)
- **Purpose**: Document analysis, MCQ generation, summaries
- **Get it from**: [Google AI Studio](https://makersuite.google.com/app/apikey)
- **Free tier**: Yes, generous limits
- **Add to .env**: `VITE_GEMINI_API_KEY=your_key_here`

### 2. OCR.space API Key (Required for Handwritten Notes)
- **Purpose**: Extract text from images and handwritten notes
- **Get it from**: [OCR.space](https://ocr.space/ocrapi)
- **Free tier**: Yes, 25,000 requests/month
- **Add to .env**: `VITE_OCR_API_KEY=your_key_here`

### 3. Text-to-Speech API Key (Optional - for Voice Assistant)
- **Purpose**: Voice responses and audio feedback
- **Get it from**: Choose a TTS provider (Google Cloud TTS, Amazon Polly, etc.)
- **Add to .env**: `VITE_TTS_API_KEY=your_key_here`

## 📝 Your .env File Should Look Like This

```env
# Supabase (Already configured)
VITE_SUPABASE_URL=https://wjeladftdrfvlhlcbrox.supabase.co
VITE_SUPABASE_ANON_KEY=your_existing_key

# AI Services (You need to add these)
VITE_GEMINI_API_KEY=your_gemini_api_key_here
VITE_OCR_API_KEY=your_ocr_space_api_key_here
VITE_TTS_API_KEY=your_tts_api_key_here
```

## 🎯 How to Get Started

### Step 1: Get Your API Keys
1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey) and create a Gemini API key
2. Visit [OCR.space](https://ocr.space/ocrapi) and sign up for a free API key
3. (Optional) Get a TTS API key from your preferred provider

### Step 2: Update Your .env File
1. Open the `.env` file in your project root
2. Add the API keys you obtained
3. Save the file

### Step 3: Run the App
```bash
npm install
npm run dev -- --host 127.0.0.1
```

### Step 4: Sign Up
1. Open the app in your browser
2. Click "Sign Up" or "Sign in with Google"
3. Create your account
4. Start studying!

## 🎮 Features You Can Use Right Away

### Without API Keys:
- ✅ Study Timer - Track your study sessions
- ✅ Dashboard - View your progress and stats
- ✅ Profile - Manage your account
- ✅ Gamification - Earn XP, level up, maintain streaks

### With API Keys:
- ✅ AI Analysis - Upload documents and get AI insights
- ✅ OCR Processing - Extract text from handwritten notes
- ✅ MCQ Generation - Auto-generate practice questions
- ✅ Summaries - Get AI-powered summaries of your notes

## 🔧 Troubleshooting

### "AI Analysis not working"
- Check that you've added `VITE_GEMINI_API_KEY` to your `.env` file
- Restart the development server after adding the key
- Verify the API key is valid

### "OCR not working"
- Check that you've added `VITE_OCR_API_KEY` to your `.env` file
- Verify you haven't exceeded the free tier limits
- Make sure the image is clear and readable

### "Can't sign in with Google"
- Make sure you're using the correct Supabase project
- Check that Google OAuth is enabled in Supabase dashboard
- Verify the redirect URLs are configured correctly

## 📚 Next Steps

1. **Add Subjects**: Create your study subjects in the Study Timer
2. **Start Studying**: Use the timer to track your first session
3. **Upload Notes**: Try the AI Analysis feature with your study materials
4. **Track Progress**: Check your dashboard to see your stats
5. **Earn Achievements**: Keep studying to unlock achievements!

## 🎨 Customization

### Change Theme Colors
Edit `src/index.css` to customize the color scheme:
- `--primary`: Main brand color (currently blue)
- `--secondary`: Secondary color (currently green)
- `--accent`: Accent color (currently orange)

### Add More Features
Check `TODO.md` for planned features and implementation status.

## 💡 Tips for Best Experience

1. **Study Daily**: Maintain your streak for bonus XP
2. **Use Tags**: Tag sessions with difficulty and importance
3. **Upload Notes**: Let AI help you study more efficiently
4. **Set Goals**: Track your progress towards your study goals
5. **Enable Dark Mode**: Reduce eye strain during late-night study sessions

## 🆘 Need Help?

- Check the [README.md](./README.md) for detailed documentation
- Review [TODO.md](./TODO.md) for feature status
- Refer to the [Miaoda Documentation](https://intl.cloud.baidu.com/en/doc/MIAODA/)

---

Happy Studying! 📚✨
