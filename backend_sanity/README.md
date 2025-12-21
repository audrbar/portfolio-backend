# Portfolio Backend - Sanity CMS

This is the backend content management system for the portfolio website, built with Sanity.io. It provides a real-time content editing environment for managing all portfolio data.

## 🎯 Overview

Sanity Studio is an open-source, real-time content management system that powers the portfolio website. It allows for easy content updates without touching the code.

## 📋 Content Schemas

The backend includes the following content types:

### 📝 **Abouts** (`abouts.js`)
- Personal information
- Biography and description
- Profile images

### 🎯 **Skills** (`skills.js`)
- Technical skills
- Proficiency levels
- Skill icons/images

### 💼 **Works** (`works.js`)
- Portfolio projects
- Project descriptions
- Images and screenshots
- Project links
- Technologies used

### 👔 **Work Experience** (`workExperience.js`)
- Employment history
- Job titles and companies
- Dates and descriptions
- Achievements

### 💬 **Testimonials** (`testimonials.js`)
- Client feedback
- Recommendations
- Testimonial images
- Company/person details

### 🏢 **Brands** (`brands.js`)
- Technology logos
- Tools and frameworks
- Brand images

### 📧 **Contact** (`contact.js`)
- Contact form submissions
- Email addresses
- Social media links

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Sanity account

### Installation

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Initialize Sanity project** (if not already done)
   ```bash
   sanity init
   ```

3. **Start the development server**
   ```bash
   npm start
   ```
   The studio will be available at [http://localhost:3333](http://localhost:3333)

### Building for Production

```bash
npm run build
```

## 📁 Project Structure

```
backend_sanity/
├── schemas/              # Content type definitions
│   ├── schema.js         # Schema aggregator
│   ├── abouts.js         # About section
│   ├── brands.js         # Brand/tech logos
│   ├── contact.js        # Contact information
│   ├── experiences.js    # Experience data
│   ├── skills.js         # Skills and expertise
│   ├── testimonials.js   # Testimonials/reviews
│   ├── workExperience.js # Work history
│   └── works.js          # Portfolio projects
│
├── config/               # Sanity configuration
│   └── @sanity/
│       ├── data-aspects.json
│       ├── default-layout.json
│       ├── default-login.json
│       ├── form-builder.json
│       └── vision.json
│
├── static/               # Static assets
├── sanity.json           # Sanity project config
└── package.json          # Dependencies
```

## 🔧 Configuration

### API Access

The frontend connects to this Sanity backend using:
- **Project ID**: Found in `sanity.json`
- **Dataset**: Usually "production"
- **API Version**: Format `YYYY-MM-DD`

### CORS Settings

Configure CORS in your Sanity project dashboard:
1. Go to [sanity.io/manage](https://sanity.io/manage)
2. Select your project
3. Navigate to Settings → API
4. Add your frontend URL to allowed origins

## 📊 Content Management

### Adding New Content Types

1. Create a new schema file in `schemas/`
2. Define your schema structure
3. Import and add it to `schemas/schema.js`
4. Restart the Sanity Studio

### Example Schema Structure

```javascript
export default {
  name: 'contentType',
  title: 'Content Type',
  type: 'document',
  fields: [
    {
      name: 'title',
      title: 'Title',
      type: 'string',
    },
    // ... more fields
  ]
}
```

## 🛠️ Customization

### Adding Plugins

Install Sanity plugins via npm:
```bash
npm install @sanity/plugin-name
```

Then add to `sanity.json`:
```json
{
  "plugins": [
    "@sanity/plugin-name"
  ]
}
```

### Custom Components

Create custom input components in the `components/` directory and reference them in your schemas.

## 🌐 Deployment

Deploy your Sanity Studio:

```bash
sanity deploy
```

Your studio will be hosted at: `https://your-project.sanity.studio`

## 📚 Resources

- [Sanity Documentation](https://www.sanity.io/docs)
- [Schema Types](https://www.sanity.io/docs/schema-types)
- [GROQ Query Language](https://www.sanity.io/docs/groq)
- [Sanity Community](https://slack.sanity.io/)

## 🔑 Environment Variables

Required environment variables (in production):
```
SANITY_STUDIO_API_PROJECT_ID=your_project_id
SANITY_STUDIO_API_DATASET=production
```

## 👤 Author
- GitHub: [@audrbar](https://github.com/audrbar)

## 📄 License

UNLICENSED - Private project

## 🤝 Support

For Sanity-specific issues:
- [Sanity Documentation](https://www.sanity.io/docs)
- [Community Slack](https://slack.sanity.io/)
- [GitHub Issues](https://github.com/sanity-io/sanity)
