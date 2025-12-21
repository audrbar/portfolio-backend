# Portfolio Website

A modern, full-stack portfolio website showcasing projects, skills, and experience. Built with React frontend and Sanity CMS backend for dynamic content management.

## 🌟 Overview

This portfolio project consists of two main parts:
- **Frontend**: React application with smooth animations and responsive design
- **Backend**: Sanity CMS for content management

## 🚀 Live Demo

- **Website**: [Your Portfolio URL]
- **Backend**: https://github.com/audrbar/portfolio-backend
- **Frontend**: https://github.com/audrbar/portfolio-frontend

## 📦 Project Structure

```
portfolio/
├── backend_sanity/          # Sanity CMS backend
│   ├── schemas/             # Content schemas
│   └── config/              # Sanity configuration
│
└── frontend_react/          # React frontend
    ├── src/
    │   ├── components/      # Reusable components
    │   ├── container/       # Page sections
    │   └── assets/          # Static files
    └── public/
```

## 🛠️ Tech Stack

### Frontend
- React 18
- SCSS/Sass
- Framer Motion (animations)
- React Icons
- Sanity Client

### Backend
- Sanity.io CMS
- Content schemas for:
  - About information
  - Skills & expertise
  - Work projects
  - Testimonials
  - Work experience
  - Contact details

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Sanity account (for CMS)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/audrbar/portfolio.git
   cd portfolio
   ```

2. **Set up Backend**
   ```bash
   cd backend_sanity
   npm install
   npm start
   ```
   The Sanity Studio will run on [http://localhost:3333](http://localhost:3333)

3. **Set up Frontend**
   ```bash
   cd ../frontend_react
   npm install
   npm start
   ```
   The app will run on [http://localhost:3000](http://localhost:3000)

### Environment Variables

Create `.env` files in the frontend directory:
```env
REACT_APP_SANITY_PROJECT_ID=your_project_id
REACT_APP_SANITY_TOKEN=your_token
```

## 📚 Documentation

- [Backend Documentation](./backend_sanity/README.md) - Sanity CMS setup and schemas
- [Frontend Documentation](./frontend_react/README.md) - React app structure and components

## 🎨 Features

- ✨ Smooth animations and transitions
- 📱 Fully responsive design
- 🎯 Dynamic content management
- 🚀 Optimized performance
- 🎨 Modern UI/UX
- 📊 Portfolio showcase
- 💼 Work experience timeline
- 🎓 Skills display
- 💬 Testimonials section
- 📧 Contact form

## 🚢 Deployment

### Frontend
The React app can be deployed to:
- Vercel
- Netlify
- GitHub Pages

### Backend
Sanity Studio is deployed to Sanity.io cloud platform.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author
- GitHub: [@audrbar](https://github.com/audrbar)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## ⭐ Show Your Support

Give a ⭐️ if you like this project!

---

**Note**: Each subdirectory (backend_sanity and frontend_react) has its own detailed README with specific setup instructions and documentation.
