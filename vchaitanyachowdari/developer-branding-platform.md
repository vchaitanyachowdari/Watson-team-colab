# Developer Branding Platform

<img width="1470" alt="Screenshot 2025-05-11 at 11 13 12 AM" src="https://github.com/user-attachments/assets/aafe491f-1ff9-4bfd-8c0a-000f39d01ce2" />

> **Live Demo**: [https://developer-branding-platform.vercel.app](https://developer-branding-platform.vercel.app)  
> **Author**: [V Chaitanya Chowdari](https://www.linkedin.com/in/v-chaitanya-chowdari-bb3733202)  
> **GitHub**: [vchaitanyachowdari](https://github.com/vchaitanyachowdari)

## 🚀 Overview

**Developer Branding Platform** is an open-source platform to build your personal developer brand effortlessly. It generates a stunning, dynamic GitHub Profile README with AI-integrated content, live previews, and tools to showcase your projects, blogs, skills, and coding stats.

## ✨ Features

- 🧠 **AI-powered GitHub README Generator**
- 📊 **Dynamic GitHub Stats and WakaTime Integration**
- 🧩 **Skill Tags & Tech Stack Icons**
- 📰 **Dynamic Blog Feed Integration**
- 🎨 **Live Markdown Preview and Export**
- 📎 **Social Media Links & Dev Badges**
- 📤 **One-click Export to GitHub**
- 🧪 Built with **Next.js 14**, **Tailwind CSS**, and **ShadCN/UI**

## 🧰 Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Styling**: Tailwind CSS
- **UI Components**: ShadCN/UI, Lucide Icons
- **Authentication**: NextAuth.js (optional)
- **State Management**: Zustand
- **API & Tools**: GitHub API, WakaTime API, RSS Parser
- **Deployment**: Vercel

## 📁 Folder Structure

```bash
📦developer-branding-platform
├── app
│   ├── api
│   ├── dashboard
│   ├── editor
│   └── layout.tsx
├── components
│   ├── builder
│   ├── ui
│   └── shared
├── lib
│   ├── github.ts
│   ├── wakatime.ts
│   └── rss.ts
├── public
├── styles
├── types
├── utils
├── middleware.ts
└── tailwind.config.ts
```

## 🧪 How It Works

1. **Input Info**: User enters their GitHub username, skills, and social links.
2. **AI Generator**: GPT prompts generate personalized README content.
3. **Markdown Builder**: User selects what sections to include.
4. **Live Preview**: Instantly preview README content.
5. **Export**: Copy to clipboard or auto-deploy to GitHub.

## 🛠️ Getting Started

### Prerequisites

- Node.js 18+
- GitHub Token (for GitHub API)

### Installation

```bash
git clone https://github.com/vchaitanyachowdari/developer-branding-platform.git
cd developer-branding-platform
pnpm install
```

### Run Locally

```bash
pnpm dev
```

### Environment Variables

Create a `.env.local` file and add the following:

```env
GITHUB_TOKEN=your_github_token
NEXT_PUBLIC_BASE_URL=http://localhost:3000
```

> Optionally add WakaTime and Blog RSS URL for full feature support.

## ✍️ Customization

You can customize theme, layout, and sections from the `components/builder` folder.

- Edit `EditorBuilder.tsx` to change section behavior
- Update `prompts.ts` to modify AI prompt templates
- Modify Tailwind config for custom theming

## 📦 Deployment

This app is ready to deploy on Vercel.

```bash
vercel --prod
```

## 🤝 Contributing

Contributions are welcome! Here's how:

1. Fork the repository
2. Create your branch: `git checkout -b feature-name`
3. Commit changes: `git commit -m 'Add some feature'`
4. Push to branch: `git push origin feature-name`
5. Create a pull request

## 🧠 Ideas for Future

- Add dark mode toggle
- Export to PDF/PNG
- AI-powered blog writer
- Custom domain integration for hosting portfolios

## 📝 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

---

Made with 💻 by [V Chaitanya Chowdari](https://chowdari.in)

Follow me on:

- [Instagram](https://www.instagram.com/vchaitanyachowdari?utm_source=qr)
- [LinkedIn](https://www.linkedin.com/in/v-chaitanya-chowdari-bb3733202)
- [GitHub](https://github.com/vchaitanyachowdari)
- [YouTube](https://youtube.com/@vchaitanyachowdari3106)
- [Twitter](https://x.com/vchaitanyachai?s=11)
