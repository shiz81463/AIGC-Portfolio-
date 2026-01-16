# Portfolio Showcase

A beautiful, modern portfolio website built with React and Vite. Perfect for designers and creatives to showcase their work.

## Features

- 🎨 **Modern Design** - Clean, minimalist design with smooth animations
- 📱 **Fully Responsive** - Works beautifully on all devices
- ⚡ **Fast Performance** - Built with Vite for lightning-fast development and builds
- 🎯 **Smooth Navigation** - Smooth scrolling and active section highlighting
- 💫 **Animations** - Subtle animations and transitions throughout

## Sections

- **Hero** - Eye-catching introduction with call-to-action buttons
- **About** - Personal introduction and skills showcase
- **Projects** - Grid layout for showcasing your work
- **Contact** - Contact form and social links

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Navigate to the project directory:
```bash
cd portfolio-showcase
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:5173`

## Customization

### Update Your Information

1. **Hero Section** - Edit the text in `src/App.jsx`:
   - Change the title and subtitle in the Hero section
   - Update button text if needed

2. **About Section** - Modify:
   - Your bio and description
   - Skills and their progress percentages

3. **Projects** - Replace the placeholder projects:
   - Update project titles and descriptions
   - Add your project images (replace the placeholder divs)
   - Modify project tags

4. **Contact** - Update:
   - Your email address
   - Social media links (Dribbble, Behance, LinkedIn, Instagram)

### Styling

- **Colors** - Edit CSS variables in `src/index.css`:
  ```css
  --primary-color: #6366f1;
  --secondary-color: #8b5cf6;
  ```

- **Fonts** - The project uses Inter font from Google Fonts. You can change it in `index.html`

### Adding Project Images

Replace the placeholder divs in the Projects section with actual images:

```jsx
<div className="project-image">
  <img src="/path-to-your-image.jpg" alt="Project Name" />
</div>
```

## Build for Production

```bash
npm run build
```

The built files will be in the `dist` directory, ready to deploy to any static hosting service.

## Deployment

You can deploy this portfolio to:

- **Vercel** - Connect your GitHub repo for automatic deployments
- **Netlify** - Drag and drop the `dist` folder or connect via Git
- **GitHub Pages** - Use the `gh-pages` package
- **Any static hosting** - Upload the `dist` folder contents

## Technologies Used

- React 19
- Vite 7
- CSS3 (with custom properties and animations)
- Inter Font (Google Fonts)

## License

Feel free to use this template for your own portfolio!

---

**Happy designing! 🎨**
