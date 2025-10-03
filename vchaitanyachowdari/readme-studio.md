# Readme Studio

<p align="center">
  <img src="public/logo.png" alt="Readme Studio Logo" width="120" height="120">
</p>

<p align="center">
  Let AI do the writing. Readme Studio creates meaningful, professional READMEs tailored to your project and fully editable.
</p>

<p align="center">
  <a href="https://github.com/vchaitanyachowdari/readme-studio/blob/main/LICENSE.md">
    <img src="https://img.shields.io/github/license/vchaitanyachowdari/readme-studio" alt="License">
  </a>
  <a href="https://github.com/vchaitanyachowdari/readme-studio/issues">
    <img src="https://img.shields.io/github/issues/vchaitanyachowdari/readme-studio" alt="Issues">
  </a>
  <a href="https://github.com/vchaitanyachowdari/readme-studio/pulls">
    <img src="https://img.shields.io/github/issues-pr/vchaitanyachowdari/readme-studio" alt="Pull Requests">
  </a>
</p>

## 🌟 Features

Readme Studio is a powerful web application that helps developers generate professional README files effortlessly. Key features include:

- **AI-powered README Generation**: Leverages Google Gemini AI to create tailored README content based on your project details
- **Interactive Markdown Editor**: Real-time editing capabilities with a user-friendly interface
- **Live Markdown Preview**: See changes as you type with an accurate preview of your README
- **Pre-built README Templates**: Choose from a variety of templates for different project types
- **Dark/Light Mode**: Toggle between themes for comfortable editing in any lighting condition
- **Multi-step Wizard**: Guided process for collecting project information before AI generation
- **Responsive Design**: Works seamlessly across desktop and mobile devices
- **Export Functionality**: Download your generated README as a Markdown file

## 🛠️ Tech Stack

This project is built with modern web technologies:

- **[Vue 3](https://vuejs.org/)** (v3.5.17) - Progressive JavaScript framework with Composition API
- **[TypeScript](https://www.typescriptlang.org/)** (~5.8.3) - Typed superset of JavaScript
- **[Vite](https://vitejs.dev/)** (v7.0.4) - Fast build tool and development server
- **[Pinia](https://pinia.vuejs.org/)** (v3.0.3) - Intuitive, type-safe state management
- **[Vue Router](https://router.vuejs.org/)** (v4.5.1) - Official router for Vue.js applications
- **[Tailwind CSS](https://tailwindcss.com/)** (v4.1.11) - Utility-first CSS framework
- **[Marked](https://marked.js.org/)** (v16.1.1) - Markdown parser and compiler
- **[DOMPurify](https://github.com/cure53/DOMPurify)** (v3.2.6) - DOM-only, super-fast, uber-tolerant XSS sanitizer
- **[Google Generative AI](https://github.com/google/generative-ai-js)** (v0.24.1) - SDK for Google's Gemini AI models

## 📦 Installation

Follow these steps to set up the project locally:

### Prerequisites

- [Node.js](https://nodejs.org/) (version 16 or higher)
- npm (comes with Node.js) or [yarn](https://yarnpkg.com/)

### Steps

1. **Clone the repository**

```bash
git clone https://github.com/vchaitanyachowdari/readme-studio.git
cd readme-studio
```

2. **Install dependencies**

```bash
npm install
```

3. **Set up environment variables**

Create a `.env` file in the root directory and add your Google Gemini API key:

```bash
cp .env.example .env
```

Then edit the `.env` file and add your API key:

```
VITE_GOOGLE_API_KEY=your_google_gemini_api_key_here
```

> Note: The AI-powered README generation feature requires a valid Google Gemini API key. Without it, only the editor functionality will be available.

4. **Start the development server**

```bash
npm run dev
```

The application will be available at `http://localhost:5173`

## 🚀 Production Build

To create and preview a production build:

### Build the application

```bash
npm run build
```

This will generate optimized static assets in the `dist/` directory.

### Preview the production build

```bash
npm run preview
```

This serves the built app locally for testing at `http://localhost:4173`

## 📁 Project Structure

```
├── public/                 # Static assets
├── src/
│   ├── components/         # Reusable UI components
│   │   ├── editor-box/     # Editor and preview components
│   │   ├── generation-steps/ # AI generation wizard steps
│   │   ├── modals/         # Modal dialogs
│   │   ├── templates/      # Template components
│   │   └── ui/             # Custom UI components
│   ├── constants/          # Application constants
│   ├── data/               # Static data files
│   ├── layouts/            # Layout components
│   ├── pages/              # Page components (routes)
│   ├── stores/             # Pinia stores for state management
│   ├── utils/              # Utility functions
│   ├── App.vue             # Root component
│   ├── main.ts             # Entry point
│   ├── router.ts           # Vue Router configuration
│   └── style.css           # Global styles
├── index.html              # Main HTML file
├── package.json            # Project dependencies and scripts
├── tsconfig.json           # TypeScript configuration
├── vite.config.ts          # Vite configuration
└── README.md               # This file
```

## 🤝 Contributing

We welcome contributions from the community! Please read our [Contributing Guide](CONTRIBUTING.md) for details on how to:

- Report bugs and suggest features
- Submit pull requests
- Set up your development environment
- Follow our coding standards

Please also adhere to our [Code of Conduct](CODE_OF_CONDUCT.md) in all interactions.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.md) file for details.

## 🌟 Show Your Support

If you find Readme Studio helpful, please consider:

- Giving it a star on GitHub ⭐
- Sharing it with your developer friends
- Contributing to the project

## 📞 Contact

For questions, suggestions, or issues:

- Create an issue on [GitHub](https://github.com/vchaitanyachowdari/readme-studio/issues)
- Contact the maintainer: [vchaitanya@chowdari.in](mailto:vchaitanya@chowdari.in)

## 🙏 Acknowledgements

- [Google Gemini](https://ai.google.dev/) for powering the AI generation
- [Vue.js](https://vuejs.org/) for the amazing framework
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- All the open-source libraries and tools that made this project possible
