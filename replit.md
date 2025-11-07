# Doctor Profile Page Project

## Overview
A modern, responsive doctor profile page built with React and Vite. This project showcases comprehensive doctor information, credentials, services, and social media integration with Instagram and YouTube posts.

## Project Status
- **Created**: November 7, 2024
- **Migrated to React**: November 7, 2024
- **Status**: Complete and functional
- **Current Version**: 2.0.0 (React)

## Architecture

### Technology Stack
- **Frontend**: React 19 with Vite 7
- **Build Tool**: Vite (lightning-fast HMR)
- **Server**: Vite dev server on port 5000
- **Styling**: CSS3 with CSS custom properties
- **Icons**: Font Awesome 6
- **Port**: 5000 (configured for Replit webview with host 0.0.0.0)
- **Responsive**: Mobile-first design with breakpoints for tablet and desktop

### File Structure
```
react-app/
├── src/
│   ├── components/          # React components
│   │   ├── Header.jsx
│   │   ├── Navigation.jsx
│   │   ├── AboutSection.jsx
│   │   ├── EducationSection.jsx
│   │   ├── ExperienceSection.jsx
│   │   ├── ServicesSection.jsx
│   │   ├── SocialSection.jsx
│   │   └── Footer.jsx
│   ├── data/
│   │   └── doctorData.js    # Centralized data configuration
│   ├── hooks/
│   │   └── useRevealOnScroll.js
│   ├── App.jsx              # Main application component
│   ├── main.jsx             # Entry point
│   └── styles.css           # Complete styling
├── index.html
├── vite.config.js           # Vite configuration (port 5000, host 0.0.0.0)
└── package.json
```

### Key Features Implemented

1. **Component Architecture**
   - Modular React components for each section
   - Reusable components with props
   - Custom hooks for scroll animations
   - Centralized data management

2. **Profile Header**
   - Doctor photo with availability badge
   - Name, specialty, credentials
   - Quick stats (patients, rating, awards)
   - Call-to-action buttons with click handlers

3. **Tab Navigation**
   - React state management for active tab
   - Smooth scroll to content section
   - Responsive mobile-friendly tabs
   - Five main sections: About, Education, Experience, Services, Social

4. **Content Sections**
   - About: Bio, specializations, contact info, office hours
   - Education: Timeline of degrees and certifications
   - Experience: Work history and awards
   - Services: Service cards with icons and descriptions
   - Social: Social media links, Instagram posts, YouTube videos

5. **Social Media Integration**
   - Clickable links to all major social platforms
   - Instagram post feed with real URLs
   - YouTube video showcase with real URLs
   - Posts/videos open in new tabs when clicked
   - Visual indicators for video vs. image posts

6. **Interactive Features**
   - Tab navigation with active states
   - Scroll-based reveal animations
   - Click handlers for posts, videos, and buttons
   - Responsive design with touch support

7. **Responsive Design**
   - Mobile-first CSS approach
   - Breakpoints: 480px, 768px, 1024px
   - Flexible grid layouts
   - Touch-friendly interface

## Recent Changes

### November 7, 2024
- **Migration to React**: Converted vanilla HTML/CSS/JS to React components
- **Vite Setup**: Configured Vite with port 5000 and host 0.0.0.0 for Replit
- **Component Structure**: Created 8 main components (Header, Navigation, 5 sections, Footer)
- **Data Centralization**: Moved all content to `doctorData.js` for easy customization
- **Custom Hooks**: Implemented `useRevealOnScroll` for scroll animations
- **State Management**: Added React state for tab navigation
- **Workflow Update**: Updated to run Vite dev server
- **Documentation**: Created comprehensive README for React version
- **Backup**: Preserved original vanilla version in `vanilla-backup/` directory

### Previous (Vanilla Version - Nov 7, 2024)
- Initial project creation with vanilla HTML/CSS/JS
- Fixed social media links to use actual URLs
- Added data-post-url and data-video-url attributes for clickable posts/videos
- Created comprehensive customization guide

## User Preferences
- User wants modern, professional design ✅
- User wants all important details visible in one view ✅
- User wants social media integration with ability to link doctor's posts ✅
- User wants responsive design for both desktop and mobile ✅
- User requested React version ✅

## Customization Instructions

### To Update Doctor Information
1. Edit `react-app/src/data/doctorData.js`
2. Update the `doctorInfo` object with new name, specialty, credentials, etc.
3. Replace image URL with actual doctor photo
4. Update statistics, contact info, office hours

### To Add/Update Content
1. **Education**: Edit `education` array in `doctorData.js`
2. **Experience**: Edit `experience` and `awards` arrays
3. **Services**: Edit `services` array with icon, title, description
4. **Insurance**: Edit `insurance` array

### To Update Social Media
1. **Social Links**: Edit `socialLinks` array with actual URLs
2. **Instagram Posts**: Edit `instagramPosts` array with real post URLs
3. **YouTube Videos**: Edit `youtubeVideos` array with real video URLs
4. Posts/videos will automatically open in new tabs when clicked

### To Customize Styling
1. Edit `react-app/src/styles.css`
2. Modify CSS custom properties in `:root` selector
3. Update component-specific styles as needed

### To Add Features
1. Create new component in `react-app/src/components/`
2. Import and use in `App.jsx`
3. Add data to `doctorData.js` if needed

## Development Workflow
- **Dev Server**: `npm run dev` runs Vite dev server on port 5000
- **Build**: `npm run build` creates production build in `dist/`
- **Preview**: `npm run preview` previews production build
- **Workflow**: dev-server configured with webview output
- **HMR**: Hot Module Replacement enabled for instant updates
- **Host**: 0.0.0.0 (required for Replit environment)

## Deployment
- **Development**: Runs on Replit with Vite dev server
- **Production**: Build with `npm run build` and deploy `dist/` folder
- **Environment**: Configured for Replit with proper host and port settings

## Notes
- React version provides better maintainability and extensibility
- Data is centralized in `doctorData.js` for easy updates
- Original vanilla version preserved in `vanilla-backup/` for reference
- All social media links and posts are functional with real URLs
- Images use Unsplash for demonstration - should be replaced with real content
- Component-based architecture makes it easy to add/remove sections

## Version History
- **v2.0.0** (Nov 7, 2024): React migration with Vite
- **v1.0.0** (Nov 7, 2024): Initial vanilla HTML/CSS/JS version
