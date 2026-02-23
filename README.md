# Hackathon Phase 4 - Full Stack Application

A modern full-stack web application built with **Next.js** (Frontend) and **Python/Node.js** (Backend), designed for hackathon Phase 4.

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ and npm
- Python 3.8+ (for backend)
- Git

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/BinteZain/-Hackathon_2_Phase_4-.git
cd "-Hackathon_2_Phase_4-"
```

2. **Install Frontend Dependencies**
```bash
cd frontend
npm install
```

3. **Setup Environment Variables**
```bash
# Create .env.local in frontend directory
cp .env.example .env.local
```

## 📁 Project Structure

```
.
├── frontend/              # Next.js frontend application
│   ├── app/              # Next.js 13+ app directory
│   ├── components/       # React components
│   ├── public/           # Static assets
│   ├── styles/           # Global styles
│   └── package.json      # Frontend dependencies
├── backend/              # Python/Node.js backend
│   ├── main.py          # Main backend entry point
│   └── requirements.txt # Python dependencies
├── specs/               # Specification documents
├── history/             # Project history and records
├── vercel.json          # Vercel deployment configuration
└── README.md            # This file
```

## 🛠️ Development

### Frontend Development

```bash
cd frontend
npm run dev
```

The app will be available at `http://localhost:3000`

### Backend Development

```bash
# Python backend
python main.py

# Or using run script
python run_backend.py
```

## 🌐 Deployment

### Vercel Deployment (Frontend)

This project is pre-configured for Vercel deployment.

1. **Install Vercel CLI** (optional)
```bash
npm install -g vercel
```

2. **Deploy to Vercel**
```bash
# Using Vercel CLI
vercel

# Or connect your GitHub repository at vercel.com
# Vercel will automatically detect the configuration
```

3. **Environment Variables on Vercel**

Add the following environment variables in your Vercel project settings:

- `NEXT_PUBLIC_API_URL` - Your backend API URL
- `NEXT_PUBLIC_BETTER_AUTH_SECRET` - Authentication secret key

### Backend Deployment

Deploy the backend separately to your preferred platform (Heroku, Railway, Render, etc.)

## 🔧 Configuration

### Vercel Configuration

The `vercel.json` file contains:

- Build commands
- Output directory configuration
- Environment variables
- Rewrite rules for API calls
- Redirects

### Environment Variables

Create a `.env.local` file in the `frontend` directory:

```env
NEXT_PUBLIC_API_URL=http://localhost:8000/api/v1
NEXT_PUBLIC_BETTER_AUTH_SECRET=your-secret-key-here
```

## 📦 Features

- ✅ Modern Next.js 13+ frontend
- ✅ Responsive UI design
- ✅ API integration
- ✅ Authentication support
- ✅ TypeScript support
- ✅ Tailwind CSS styling
- ✅ Ready for Vercel deployment

## 🧪 Testing

```bash
# Frontend tests
cd frontend
npm test

# Linting
npm run lint
```

## 📝 Scripts

### Frontend Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |

## ⚠️ Important Notes

- **DO NOT commit `node_modules/`** - It's excluded in `.gitignore`
- **DO NOT commit `.env` files** - Keep secrets secure
- **DO NOT commit `.next/`** - Build artifacts are excluded
- Always run `npm install` after pulling changes

## 🤝 Contributing

1. Create a feature branch
2. Make your changes
3. Test thoroughly
4. Submit a pull request

## 📄 License

This project is part of Hackathon Phase 4.

## 🔗 Links

- **GitHub Repository**: https://github.com/BinteZain/-Hackathon_2_Phase_4-
- **Vercel Documentation**: https://vercel.com/docs

## 🆘 Troubleshooting

### Build Errors on Vercel

1. Ensure all dependencies are in `package.json`
2. Check that `vercel.json` build commands are correct
3. Verify environment variables are set in Vercel dashboard

### Module Not Found

```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install
```

### API Connection Issues

- Verify `NEXT_PUBLIC_API_URL` is correctly set
- Check CORS configuration on backend
- Ensure backend is running and accessible

---

**Built with ❤️ for Hackathon Phase 4**
