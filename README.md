# ContentGenAI - AI-Powered Social Media Content Generator

A full-stack SaaS prototype that helps creators, brands, and marketers generate, optimize, personalize, and analyze digital content across social platforms using AI.

## 🚀 Features

- **AI Content Generation**: Create engaging captions, hashtags, and content ideas
- **Multi-Platform Support**: Instagram, LinkedIn, and Twitter optimization
- **Engagement Prediction**: AI-powered engagement scoring (1-10 scale)
- **Content Optimization**: Improve existing content for better performance
- **Post Preview**: See how your content looks on different platforms
- **Content Library**: Save and manage all your generated posts
- **Analytics Dashboard**: Track performance and get insights
- **Visual Suggestions**: AI-recommended visual content ideas

## 🛠️ Tech Stack

### Frontend
- **Next.js 14** - React framework with App Router
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Lucide React** - Beautiful icons

### Backend
- **Next.js API Routes** - Serverless API endpoints
- **Local Storage** - Client-side data persistence (MVP)

### AI Integration
- **OpenAI API** - Content generation (with mock fallback)
- **Custom AI Prompts** - Optimized for social media content

## 📦 Installation & Setup

### Prerequisites
- **Node.js 18+** - [Download from nodejs.org](https://nodejs.org/)
- **npm** (comes with Node.js)

### Quick Start

1. **Install Node.js** (if not already installed)
   - Go to [nodejs.org](https://nodejs.org/)
   - Download and install the LTS version
   - Restart your terminal after installation

2. **Verify Installation**
   ```bash
   node --version
   npm --version
   ```

3. **Clone and Setup Project**
   ```bash
   # Navigate to project directory
   cd contentgenai
   
   # Install dependencies
   npm install
   
   # Start development server
   npm run dev
   ```

4. **Open Application**
   - Open [http://localhost:3000](http://localhost:3000) in your browser
   - Start creating AI-powered content!

### Environment Setup (Optional)

For real AI features (otherwise uses mock data):

```bash
# Copy environment file
cp .env.example .env.local

# Edit .env.local with your OpenAI API key
OPENAI_API_KEY=your_openai_api_key_here
```

## 🎯 User Flow

1. **Dashboard** (`/`) - Overview of your content performance
2. **Generate** (`/generate`) - Create new content with AI
   - Enter topic, platform, tone, and target audience
   - Get AI-generated ideas, captions, and hashtags
   - Receive engagement predictions
   - Get optimized versions
3. **Preview** (`/preview`) - See how posts look on different platforms
4. **Saved Posts** (`/saved`) - Manage your content library
5. **Analytics** (`/analytics`) - Track performance and insights

## 📱 API Endpoints

### Content Generation
- `POST /api/generate-caption` - Generate AI captions
- `POST /api/generate-hashtags` - Generate trending hashtags
- `POST /api/optimize-content` - Optimize existing content
- `POST /api/predict-engagement` - Predict engagement scores

### Data Management
- `GET /api/saved-posts` - Retrieve saved posts
- `POST /api/saved-posts` - Save new posts
- `DELETE /api/saved-posts` - Delete posts

## 🎨 UI Components

### Pages
- **Dashboard** (`/`) - Main overview and stats
- **Generate** (`/generate`) - Content creation interface
- **Preview** (`/preview`) - Social media post previews
- **Saved Posts** (`/saved`) - Content library management
- **Analytics** (`/analytics`) - Performance dashboard

## 🔮 AI Features

### Content Generation
- Topic-based content ideas
- Platform-optimized captions
- Trending hashtag suggestions
- Visual content recommendations

### Optimization
- Engagement score prediction
- Content improvement suggestions
- Platform-specific optimizations
- Tone and audience alignment

### Analytics
- Performance tracking
- Trend analysis
- Hashtag effectiveness
- Platform comparison

## 🚀 Deployment

### Vercel (Recommended)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Set environment variables in Vercel dashboard
```

### Other Platforms
The app can be deployed to any platform supporting Next.js:
- Netlify
- Railway
- Heroku
- AWS Amplify

## 🔧 Development Commands

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Run linting
npm run lint

# Check system requirements
npm run check
```

## 🐛 Troubleshooting

### Node.js Not Found
- Ensure Node.js is properly installed from [nodejs.org](https://nodejs.org/)
- Restart your terminal after installation
- Check PATH environment variable includes Node.js

### Port Already in Use
```bash
# Use different port
npm run dev -- -p 3001
```

### Dependencies Issues
```bash
# Clear cache and reinstall
npm cache clean --force
rm -rf node_modules package-lock.json
npm install
```

## 📊 Demo Data

The app includes mock data for demonstration:
- Sample generated content
- Fake engagement scores
- Mock analytics data
- Simulated API responses

## 🔄 Project Structure

```
contentgenai/
├── app/                    # Next.js app directory
│   ├── api/               # API routes
│   ├── generate/          # Content generation page
│   ├── preview/           # Post preview page
│   ├── saved/             # Saved posts page
│   ├── analytics/         # Analytics dashboard
│   └── globals.css        # Global styles
├── components/            # Reusable components
├── lib/                   # Utilities and helpers
├── public/               # Static assets
└── README.md
```

## 🎯 Future Enhancements

- Real database integration (PostgreSQL/MongoDB)
- User authentication and accounts
- Team collaboration features
- Advanced analytics and reporting
- Content scheduling
- Social media API integrations
- Image generation with DALL-E
- A/B testing capabilities

## 📝 License

This project is for demonstration purposes. Feel free to use and modify as needed.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📞 Support

For questions or issues:
1. Check Node.js installation: `node --version`
2. Clear npm cache: `npm cache clean --force`
3. Delete node_modules and reinstall: `rm -rf node_modules && npm install`
4. Check the console for error messages

---

**ContentGenAI** - Empowering creators with AI-driven content generation 🚀
