# Resume Builder Website Clone

A comprehensive AI-powered productivity platform that helps users transform hours of work into minutes using artificial intelligence. This project is a complete recreation of the BlinkFind website with enhanced features and a modern light theme design.

## 🌟 Overview

Resume Builder is an innovative AI platform designed for busy professionals who want to maximize their productivity. The platform offers a suite of AI-powered tools, with the flagship AI Resume Builder that creates ATS-optimized resumes in minutes.

## ✨ Features

### Core Features
- **AI Resume Builder**: Create professional, ATS-optimized resumes with AI assistance
- **Multi-step Form Process**: Comprehensive resume building with progress tracking
- **Real-time ATS Scoring**: Live feedback on resume optimization (0-100 scale)
- **Dynamic Content Management**: Add/remove multiple education, experience, and project entries
- **Progress Tracking**: Individual field completion percentages and overall progress
- **Issue Detection**: Automatic identification of missing critical sections

### Technical Features
- **Responsive Design**: Fully responsive across all device sizes
- **Modern UI/UX**: Clean, professional interface with smooth animations
- **Form Validation**: Real-time validation with progress indicators
- **Interactive Elements**: Hover effects, transitions, and dynamic content
- **Accessibility**: WCAG compliant with proper ARIA labels and keyboard navigation

## 🏗️ Architecture

### Project Structure
   ```
resume-builder/
├── app/                          # Next.js App Router
│   ├── globals.css              # Global styles and CSS variables
│   ├── layout.tsx               # Root layout component
│   ├── page.tsx                 # Homepage
│   ├── about/
│   │   └── page.tsx            # About page
│   └── resume-builder/
│       └── page.tsx            # Resume builder application
├── components/
│   ├── ui/                      # Reusable UI components
│   │   ├── button.tsx
│   │   ├── card.tsx
│   │   ├── input.tsx
│   │   ├── label.tsx
│   │   ├── textarea.tsx
│   │   ├── tabs.tsx
│   │   ├── progress.tsx
│   │   └── badge.tsx
│   └── theme-provider.tsx       # Theme management
├── lib/
│   └── utils.ts                 # Utility functions
├── public/                      # Static assets
├── styles/                      # Additional stylesheets
└── README.md                    # Project documentation
```

### Technology Stack
- **Framework**: Next.js 15.2.4 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: Radix UI primitives
- **Icons**: Lucide React
- **State Management**: React useState hooks
- **Form Handling**: Controlled components with real-time validation

## 🚀 Getting Started

### Prerequisites
- Node.js 18.0 or higher
- npm, yarn, or pnpm package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/vchaitanyachowdari/Resume-Builder.git
   cd blinkfind-clone
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

4. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000) to see the application.

### Build for Production

```bash
npm run build
npm start
```

## 📱 Pages & Components

### Homepage (\`/\`)
- **Hero Section**: Main value proposition with gradient text effects
- **Product Showcase**: AI Resume Builder feature card
- **Navigation**: Responsive navigation with login/signup buttons
- **Background Effects**: Animated gradient backgrounds

### About Page (\`/about\`)
- **Company Story**: Mission, vision, and team information
- **Feature Cards**: Interactive cards showcasing company values
- **Call-to-Action**: Conversion-focused sections

### Resume Builder (\`/resume-builder\`)
- **Multi-step Form**: Four main sections (Personal, Education, Experience, Skills)
- **Progress Tracking**: Real-time completion percentages
- **ATS Scoring**: Dynamic scoring with suggestions
- **Form Management**: Add/remove dynamic entries

## 🎨 Design System

### Color Palette (Light Theme)
```css
/* Primary Colors */
--primary: #6366f1        /* Indigo-500 */
--primary-foreground: #ffffff

/* Background Colors */
--background: #ffffff     /* White */
--card: #f8fafc          /* Slate-50 */
--muted: #f1f5f9         /* Slate-100 */

/* Text Colors */
--foreground: #0f172a    /* Slate-900 */
--muted-foreground: #64748b /* Slate-500 */

/* Accent Colors */
--accent: #e0e7ff        /* Indigo-100 */
--secondary: #f1f5f9     /* Slate-100 */
```

### Typography
- **Font Family**: Inter (system font fallback)
- **Headings**: Bold weights with proper hierarchy
- **Body Text**: Regular weight with optimal line height
- **Code**: Monospace font for technical content

### Spacing & Layout
- **Container**: Max-width with responsive padding
- **Grid System**: CSS Grid and Flexbox for layouts
- **Spacing Scale**: Consistent 4px base unit scaling

## 🔧 Component Documentation

### Button Component
```tsx
<Button variant="default" size="lg" className="custom-class">
  Click me
</Button>
```

**Variants**: default, destructive, outline, secondary, ghost, link
**Sizes**: default, sm, lg, icon

### Card Component
```tsx
<Card>
  <CardHeader>
    <CardTitle>Title</CardTitle>
    <CardDescription>Description</CardDescription>
  </CardHeader>
  <CardContent>
    Content goes here
  </CardContent>
</Card>
```

### Form Components
```tsx
<div className="space-y-2">
  <Label htmlFor="input">Label</Label>
  <Input id="input" placeholder="Enter text..." />
</div>
```

### Progress Component
```tsx
<Progress value={75} className="w-full" />
```

## 📊 Resume Builder Features

### Personal Information Section
- First Name* (Required)
- Last Name* (Required)
- Email Address* (Required)
- Phone Number
- Location
- LinkedIn Profile
- Portfolio/Website
- Professional Summary* (Required)

### Education Section
- Degree/Qualification* (Required)
- Institution/University* (Required)
- Location
- GPA (Optional)
- Start Date
- End Date
- Relevant Coursework, Projects, or Achievements

### Experience Section
- Job Title
- Company
- Location
- Start Date
- End Date
- Job Description

### Skills & Projects Section
- Skills (Technical and soft skills)
- Projects with:
  - Project Name
  - Description
  - Technologies Used

### ATS Scoring Algorithm
The ATS score is calculated based on:
- Personal information completeness (20 points)
- Professional summary quality (30 points)
- Education details (20 points)
- Work experience (20 points)
- Skills section (10 points)

## 🔄 State Management

### Form Data Structure
```typescript
interface FormData {
  firstName: string
  lastName: string
  email: string
  phone: string
  location: string
  linkedin: string
  portfolio: string
  summary: string
  education: EducationEntry[]
  experience: ExperienceEntry[]
  skills: string
  projects: ProjectEntry[]
}
```

### Progress Calculation
- Individual field progress: 0% (empty) or 100% (filled)
- Overall progress: Percentage of required fields completed
- Section progress: Calculated per form section

## 🎯 User Experience Features

### Interactive Elements
- **Hover Effects**: Smooth transitions on buttons and cards
- **Focus States**: Clear focus indicators for accessibility
- **Loading States**: Visual feedback during interactions
- **Error Handling**: User-friendly error messages

### Responsive Design
- **Mobile First**: Optimized for mobile devices
- **Tablet Support**: Adapted layouts for medium screens
- **Desktop Enhancement**: Full-featured desktop experience

### Accessibility
- **Keyboard Navigation**: Full keyboard support
- **Screen Reader Support**: Proper ARIA labels
- **Color Contrast**: WCAG AA compliant contrast ratios
- **Focus Management**: Logical tab order

## 🚀 Deployment

### Vercel Deployment (Recommended)
1. Connect your GitHub repository to Vercel
2. Configure build settings (auto-detected for Next.js)
3. Deploy with automatic CI/CD

### Manual Deployment
```bash
npm run build
npm run export  # For static export if needed
```

## 🧪 Testing

### Manual Testing Checklist
- [ ] All pages load correctly
- [ ] Navigation works across all pages
- [ ] Form validation functions properly
- [ ] Progress tracking updates in real-time
- [ ] ATS scoring calculates correctly
- [ ] Responsive design works on all screen sizes
- [ ] Accessibility features function properly

## 🔮 Future Enhancements

### Planned Features
- **PDF Generation**: Export resumes as PDF files
- **Template Selection**: Multiple resume templates
- **AI Content Suggestions**: Smart content recommendations
- **User Authentication**: Save and manage multiple resumes
- **Database Integration**: Persistent data storage
- **Payment Integration**: Premium features

### Technical Improvements
- **Performance Optimization**: Code splitting and lazy loading
- **SEO Enhancement**: Meta tags and structured data
- **Analytics Integration**: User behavior tracking
- **Error Monitoring**: Crash reporting and monitoring

## 🤝 Contributing

### Development Guidelines
1. Follow TypeScript best practices
2. Use consistent naming conventions
3. Write descriptive commit messages
4. Test thoroughly before submitting PRs
5. Update documentation for new features

### Code Style
- Use Prettier for code formatting
- Follow ESLint rules
- Use meaningful variable names
- Add comments for complex logic

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Original Design**: Inspired by BlinkFind.in
- **UI Components**: Built with Radix UI primitives
- **Icons**: Lucide React icon library
- **Styling**: Tailwind CSS framework

## 📞 Support

For support, email vchaitanya@chowdari.in or create an issue in the GitHub repository.

---

**Built with ❤️ using Next.js, TypeScript, and Tailwind CSS**
