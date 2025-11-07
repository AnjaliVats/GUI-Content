# Doctor Profile Page - React Version

A modern, responsive doctor profile page built with **React** and **Vite**. This application displays comprehensive doctor information, credentials, services, and social media integration.

## Features

- ⚛️ **Built with React** - Modern React with hooks and functional components
- ⚡ **Vite** - Lightning-fast development server and build tool
- 📱 **Fully Responsive** - Works seamlessly on desktop, tablet, and mobile devices
- 🎨 **Modern UI** - Clean, professional design with smooth animations
- 🔄 **Interactive** - Tab navigation, clickable posts/videos, scroll animations
- 📊 **Data-Driven** - Centralized data structure for easy customization

## What's Included

- **Comprehensive Doctor Information**:
  - Bio and credentials
  - Education and certifications
  - Professional experience and awards
  - Services offered
  - Contact information and office hours
  - Insurance providers accepted

- **Social Media Integration**:
  - Links to all major platforms (Instagram, Twitter, LinkedIn, YouTube, Facebook)
  - Instagram posts feed
  - YouTube videos showcase
  - Clickable posts/videos that open in new tabs

- **Interactive Features**:
  - Tab navigation between sections
  - Smooth scroll animations
  - Responsive mobile menu
  - Interactive buttons and cards

## Project Structure

```
.
├── react-app/               # React application directory
│   ├── src/
│   │   ├── components/      # React components
│   │   │   ├── Header.jsx
│   │   │   ├── Navigation.jsx
│   │   │   ├── AboutSection.jsx
│   │   │   ├── EducationSection.jsx
│   │   │   ├── ExperienceSection.jsx
│   │   │   ├── ServicesSection.jsx
│   │   │   ├── SocialSection.jsx
│   │   │   └── Footer.jsx
│   │   ├── data/            # Data configuration
│   │   │   └── doctorData.js
│   │   ├── hooks/           # Custom React hooks
│   │   │   └── useRevealOnScroll.js
│   │   ├── App.jsx          # Main app component
│   │   ├── main.jsx         # Entry point
│   │   └── styles.css       # All styling
│   ├── index.html
│   ├── vite.config.js       # Vite configuration
│   └── package.json
├── vanilla-backup/          # Original vanilla HTML/CSS/JS version
├── package.json             # Root package.json
└── README.md
```

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm

### Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd GUI-Content
```

2. Install dependencies:
```bash
cd react-app
npm install
```

3. Start the development server:
```bash
npm run dev
```

The app will be available at `http://localhost:5000`

## Available Scripts

From the root directory:

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## Customization Guide

### 1. Update Doctor Information

Edit `react-app/src/data/doctorData.js`:

```javascript
export const doctorInfo = {
  name: "Your Doctor Name",
  specialty: "Your Specialty",
  image: "your-image-url",
  // ... update all fields
};
```

### 2. Customize Education & Experience

Update the `education`, `experience`, and `awards` arrays in `doctorData.js`:

```javascript
export const education = [
  {
    year: "2020 - 2024",
    degree: "Your Degree",
    institution: "Your Institution",
    description: "Your description"
  },
  // ...
];
```

### 3. Modify Services

Edit the `services` array:

```javascript
export const services = [
  {
    icon: "fa-heart-pulse",  // Font Awesome icon class
    title: "Service Name",
    description: "Service description"
  },
  // ...
];
```

### 4. Update Social Media

**Social Links**: Edit `socialLinks` array in `doctorData.js`:

```javascript
export const socialLinks = [
  {
    platform: "instagram",
    url: "https://www.instagram.com/your-username",
    handle: "@YourUsername",
    icon: "fab fa-instagram"
  },
  // ...
];
```

**Instagram Posts**: Edit `instagramPosts` array:

```javascript
export const instagramPosts = [
  {
    id: 1,
    url: "https://www.instagram.com/p/YOUR_POST_ID/",
    image: "your-image-url",
    caption: "Your caption",
    likes: "1.5k",
    comments: "89",
    isVideo: false  // Set to true for video posts
  },
  // ...
];
```

**YouTube Videos**: Edit `youtubeVideos` array:

```javascript
export const youtubeVideos = [
  {
    id: 1,
    url: "https://www.youtube.com/watch?v=YOUR_VIDEO_ID",
    thumbnail: "https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg",
    title: "Video Title",
    views: "100k views",
    uploaded: "1 week ago",
    duration: "10:30"
  },
  // ...
];
```

### 5. Customize Styling

Edit `react-app/src/styles.css`. Key variables are at the top:

```css
:root {
  --primary-color: #2563eb;
  --secondary-color: #1e40af;
  --accent-color: #3b82f6;
  /* ... more variables */
}
```

### 6. Add Functionality to Buttons

Edit `react-app/src/components/Header.jsx`:

```javascript
const handleBookAppointment = () => {
  // Replace with your booking system integration
  window.location.href = 'https://your-booking-system.com';
};
```

## Deployment

### Build for Production

```bash
cd react-app
npm run build
```

The optimized files will be in `react-app/dist/`

### Deploy to Replit

The app is pre-configured to run on Replit with:
- Port: 5000
- Host: 0.0.0.0
- HMR (Hot Module Replacement) enabled

Just click "Run" in Replit!

## Technology Stack

- **React 19** - UI library
- **Vite 7** - Build tool and dev server
- **Font Awesome 6** - Icons
- **CSS3** - Styling with CSS custom properties
- **Intersection Observer API** - Scroll animations

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Migration from Vanilla Version

The original vanilla HTML/CSS/JS version is preserved in the `vanilla-backup/` directory. Key improvements in the React version:

- ✅ Component-based architecture
- ✅ Centralized data management
- ✅ Better state management
- ✅ Easier to maintain and extend
- ✅ Type-safe with potential TypeScript migration
- ✅ Better development experience with HMR

## Tips for Best Results

1. **Images**: Use high-quality images (400x400px for profile, 600x600px for posts)
2. **Performance**: Optimize images before uploading
3. **Content**: Keep descriptions concise and scannable
4. **Testing**: Test on actual mobile devices
5. **Updates**: Regularly update social media posts to keep content fresh

## License

MIT License - feel free to use and modify for your needs.

## Support

For issues or questions, please open an issue on GitHub.
