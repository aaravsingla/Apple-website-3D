# iPhone 15 Pro Landing Page

A stunning recreation of Apple's iPhone 15 Pro website featuring immersive 3D models, smooth animations, and responsive design. Built with modern web technologies to showcase the iPhone 15 Pro with interactive elements and beautiful visual effects.

## 🚀 Live Demo

[**View Live Website**](https://apple-aarav-website-3-d-9js9.vercel.app/)

## ✨ Features

- **3D Interactive Models**: Explore iPhone 15 Pro models in 3D with different colors and sizes
- **Smooth Animations**: GSAP-powered animations with scroll triggers
- **Video Carousel**: Interactive video highlights with custom controls
- **Responsive Design**: Optimized for all device sizes
- **Color Variants**: Switch between Natural, Blue, White, and Black Titanium
- **Size Options**: Toggle between 6.1" and 6.7" models
- **Performance Monitoring**: Integrated with Sentry for error tracking

## 🛠️ Built With

- **React 18** - Frontend framework
- **Three.js** - 3D graphics and modeling
- **React Three Fiber** - React renderer for Three.js
- **React Three Drei** - Useful helpers for R3F
- **GSAP** - Professional animations
- **Tailwind CSS** - Utility-first CSS framework
- **Vite** - Fast build tool
- **Sentry** - Error monitoring and performance tracking

## 📁 Project Structure

```
iphone/
├── public/
│   ├── assets/
│   │   ├── images/       # Static images
│   │   └── videos/       # Video assets
│   └── models/           # 3D model files
├── src/
│   ├── components/       # React components
│   │   ├── Features.jsx      # Titanium features section
│   │   ├── Footer.jsx        # Footer component
│   │   ├── Hero.jsx          # Hero section with video
│   │   ├── Highlights.jsx    # Video highlights carousel
│   │   ├── HowItWorks.jsx    # A17 Pro chip section
│   │   ├── IPhone.jsx        # 3D iPhone model
│   │   ├── Lights.jsx        # 3D scene lighting
│   │   ├── Loader.jsx        # Loading component
│   │   ├── Model.jsx         # 3D model showcase
│   │   ├── ModelView.jsx     # 3D model viewer
│   │   ├── Navbar.jsx        # Navigation header
│   │   └── VideoCarousel.jsx # Interactive video carousel
│   ├── constants/        # Static data and configuration
│   ├── utils/           # Utility functions and animations
│   ├── App.jsx          # Main app component
│   └── main.jsx         # App entry point
```

## 🎯 Key Components

### 3D Model Showcase
- Interactive iPhone 15 Pro models with realistic materials
- Color switching between all available variants
- Size comparison between 6.1" and 6.7" models
- Smooth rotation and camera controls

### Video Carousel
- Custom video player with progress indicators
- Smooth transitions between highlight videos
- Play, pause, and replay functionality
- Responsive design for all screen sizes

### Animated Sections
- Scroll-triggered animations using GSAP
- Smooth transitions and reveals
- Performance-optimized animations

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd iphone
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Start the development server
```bash
npm run dev
# or
yarn dev
```

4. Open your browser and navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
# or
yarn build
```

## 🎨 Customization

### Colors
Modify the color variants in `src/constants/index.js`:
```javascript
export const models = [
  {
    id: 1,
    title: "iPhone 15 Pro in Natural Titanium",
    color: ["#8F8A81", "#ffe7b9", "#6f6c64"],
    img: yellowImg,
  },
  // Add more color variants...
];
```

### Animations
Customize animations in `src/utils/animations.js` using GSAP:
```javascript
export const animateWithGsap = (target, animationProps, scrollProps) => {
  gsap.to(target, {
    ...animationProps,
    scrollTrigger: {
      // Customize scroll trigger settings
    }
  })
}
```

## 📱 Responsive Design

The website is fully responsive and optimized for:
- Desktop (1024px+)
- Tablet (768px - 1023px)
- Mobile (320px - 767px)

## 🔧 Performance Optimizations

- Lazy loading for 3D models and videos
- Optimized animations with GSAP
- Responsive image and video loading
- Efficient component rendering with React

