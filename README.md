# WeblifyAI - AI-Powered Website Builder & SEO Platform

A modern, fully responsive SaaS landing page built with React, TypeScript, and Tailwind CSS. Features dark mode UI, glassmorphism effects, and smooth animations.

## 🚀 Features

- **Modern Design**: Dark mode UI with glassmorphism effects
- **Fully Responsive**: Optimized for mobile, tablet, and desktop
- **Interactive Components**: Tabbed demo, pricing toggle, testimonial carousel
- **Smooth Animations**: Framer Motion powered animations and micro-interactions
- **SEO Optimized**: Proper semantic HTML and meta tags
- **GDPR Compliant**: Cookie consent popup with detailed information
- **AI Chatbot**: Floating chatbot interface (ready for integration)
- **Complete Routing**: Privacy policy and terms pages included

## 🛠 Tech Stack

- **Frontend**: React 18, TypeScript, Vite
- **Styling**: Tailwind CSS, Custom CSS
- **Animations**: Framer Motion
- **Icons**: Lucide React
- **Routing**: React Router DOM
- **Build Tool**: Vite

## 📦 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd weblifyai-landing
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Build for production:
```bash
npm run build
```

## 🌐 Deployment

### Vercel Deployment

1. Install Vercel CLI:
```bash
npm install -g vercel
```

2. Deploy:
```bash
vercel --prod
```

### Cloudflare Pages Deployment

1. Connect your repository to Cloudflare Pages
2. Set build settings:
   - Build command: `npm run build`
   - Build output directory: `dist`
   - Node.js version: `18.x`

### Netlify Deployment

1. Connect your repository to Netlify
2. Set build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`

## 🔧 Configuration

### Google reCAPTCHA Setup

1. Get your reCAPTCHA site key from [Google reCAPTCHA](https://www.google.com/recaptcha/)
2. Add the reCAPTCHA script to `index.html`:
```html
<script src="https://www.google.com/recaptcha/api.js" async defer></script>
```
3. Update the contact form component to include reCAPTCHA validation

### Chatbot Integration

The chatbot component is ready for integration with:
- **Dialogflow**: Add your project ID and credentials
- **Tidio**: Insert your Tidio script
- **Intercom**: Add your Intercom app ID
- **Custom AI**: Integrate with your AI endpoint

Example integration:
```javascript
// In src/components/Chatbot.tsx
const sendToAI = async (message) => {
  const response = await fetch('/api/chat', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ message })
  });
  return response.json();
};
```

### Google Maps Integration

Replace the map placeholder in `src/components/Contact.tsx`:

```javascript
// Option 1: Google Maps Embed
<iframe
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d..."
  width="100%"
  height="200"
  style={{ border: 0 }}
  allowFullScreen=""
  loading="lazy"
  referrerPolicy="no-referrer-when-downgrade"
></iframe>

// Option 2: Leaflet (React Leaflet)
npm install react-leaflet leaflet
```

## 📁 Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── Header.tsx      # Navigation header
│   ├── Hero.tsx        # Hero section
│   ├── Features.tsx    # Features showcase
│   ├── Demo.tsx        # Interactive demo
│   ├── UseCases.tsx    # Use cases section
│   ├── Pricing.tsx     # Pricing plans
│   ├── Testimonials.tsx # Customer testimonials
│   ├── Contact.tsx     # Contact form
│   ├── Footer.tsx      # Site footer
│   ├── GDPRPopup.tsx   # Cookie consent
│   └── Chatbot.tsx     # AI chatbot
├── pages/              # Page components
│   ├── LandingPage.tsx # Main landing page
│   ├── PrivacyPolicy.tsx # Privacy policy
│   └── TermsAndConditions.tsx # Terms page
├── App.tsx             # Main app component
├── main.tsx            # Entry point
└── index.css           # Global styles
```

## 🎨 Design System

### Colors
- Primary: `#22d3ee` (Cyan 400)
- Secondary: `#3b82f6` (Blue 500)
- Background: `#111827` (Gray 900)
- Cards: `#1f2937` (Gray 800)
- Text: `#f9fafb` (Gray 50)
- Muted: `#6b7280` (Gray 500)

### Typography
- Headers: JetBrains Mono (monospace)
- Body: Inter (sans-serif)
- Weights: 400, 500, 600, 700

### Spacing
- Base unit: 4px (0.25rem)
- Scale: 4, 8, 12, 16, 20, 24, 32, 40, 48, 64px

## 🔮 Future Enhancements

- **NVIDIA SDK Integration**: NeMo for natural language processing, Triton Inference Server for AI model serving
- **Advanced Analytics**: User behavior tracking and conversion analytics
- **A/B Testing**: Component variants for optimization
- **Multi-language Support**: Internationalization (i18n)
- **Advanced SEO**: Schema markup, sitemap generation
- **Performance Monitoring**: Real-time performance metrics

## 📄 License

MIT License - feel free to use this project for your own purposes.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📞 Support

For support, email support@weblifyai.com or join our Discord community.

---

Built with ❤️ by the WeblifyAI team in Sri Lanka 🇱🇰