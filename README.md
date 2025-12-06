# Luminist - AI Image Editor

Luminist is a powerful, SaaS-based AI image editing application that empowers users to transform ordinary images into stunning visuals. Built with modern web technologies, it offers a seamless blend of traditional editing tools and advanced AI capabilities directly in the browser.

## 🚀 Key Features

- **🤖 AI-Powered Transformations**: Leverage advanced AI for background removal, smart enhancements, and generative features.
- **🎨 Interactive Canvas**: Robust editing environment powered by Fabric.js for layer-based manipulation and composition.
- **📂 Smart Organization**: Create and manage multiple projects, organizing them into folders for better workflow.
- **🔐 Secure Authentication**: Enterprise-grade security and authentications via Clerk, supporting Google login and more.
- **💳 Subscription Plans**: Integrated tiered access (Free & Pro) with usage limits and tracking.
- **☁️ Cloud Processing**: High-performance image processing, storage, and optimizations using ImageKit.
- **🌓 Dark Mode**: Sleek, eye-friendly dark interface (default) with theme support.

## 🛠️ Tech Stack

**Frontend**
- **Framework**: [Next.js 15](https://nextjs.org/) (App Router)
- **Language**: JavaScript / React 19
- **Styling**: [TailwindCSS](https://tailwindcss.com/) v4, [Shadcn UI](https://ui.shadcn.com/)
- **Animations**: [Framer Motion](https://www.framer.com/motion/)
- **Canvas Engine**: [Fabric.js](http://fabricjs.com/) v6

**Backend & Data**
- **Database**: [Convex](https://www.convex.dev/) (Real-time database & backend functions)
- **Authentication**: [Clerk](https://clerk.com/)

**Services & Utilities**
- **Image Processing**: [ImageKit](https://imagekit.io/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Notifications**: Sonner

## 🏁 Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

- **Node.js**: v18 or higher
- **npm** or **yarn**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/luminist.git
   cd luminist
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Environment Setup**
   Create a `.env.local` file in the root directory and add the following variables. You will need accounts for Clerk, Convex, and ImageKit.

   ```env
   # Clerk Authentication
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
   CLERK_SECRET_KEY=sk_test_...

   # Convex Database
   CONVEX_DEPLOYMENT=...
   NEXT_PUBLIC_CONVEX_URL=https://...

   # ImageKit
   NEXT_PUBLIC_IMAGEKIT_PUBLIC_KEY=...
   IMAGEKIT_PRIVATE_KEY=...
   NEXT_PUBLIC_IMAGEKIT_URL_ENDPOINT=https://ik.imagekit.io/your_id
   ```

4. **Start the Development Server**
   ```bash
   npm run dev
   ```

   Open [http://localhost:3000](http://localhost:3000) with your browser to see the application.

## 📂 Project Structure

```bash
luminist/
├── app/                  # Next.js App Router pages and layouts
│   ├── (auth)/           # Authentication routes (login/signup)
│   ├── (main)/           # Main dashboard and project listing
│   ├── editor/           # Core image editor interface and canvas logic
│   └── api/              # API route handlers
├── components/           # Reusable UI components (buttons, dialogs, etc.)
├── convex/               # Backend API functions (queries, mutations) and schema
├── lib/                  # Utility functions and shared helpers
├── public/               # Static assets (images, icons)
└── styles/               # Global styles and CSS configurations
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

