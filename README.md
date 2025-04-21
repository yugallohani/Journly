# Journly

![Journly Banner](https://raw.githubusercontent.com/yourusername/Journly/main/public/banner.png)

A modern, privacy-focused journaling app for tracking your thoughts, moods, and memories — built with Next.js, React, Prisma, and Clerk.

---

## ✨ Features

- **User Authentication** (Clerk)
- **Rich Journal Entries** with mood tracking and image visualization
- **Collections** for organization
- **Full-text search** (optional, via Prisma)
- **Mobile-first, responsive UI** (Tailwind CSS, shadcn/ui)
- **Server-side rendering** for performance and SEO
- **Hydration-safe date rendering**
- **Dark mode**
- **Secure & private**: Your data, your control

## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/Journly.git
   cd Journly
   ```
2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```
3. **Set up environment variables**
   - Copy `.env.example` to `.env` and fill in:
     - Clerk keys
     - Database URL
     - Pixabay API key (for mood images)
     - ArcJet key (optional)
4. **Migrate and seed your database**
   ```bash
   npx prisma migrate dev
   # Optionally: npx prisma db seed
   ```
5. **Run the app**
   ```bash
   npm run dev
   # or
   yarn dev
   ```
6. **Open [http://localhost:3000](http://localhost:3000)**

---

## 🛠️ Tech Stack
- [Next.js](https://nextjs.org/)
- [React](https://react.dev/)
- [Prisma](https://prisma.io/)
- [Clerk](https://clerk.dev/)
- [date-fns](https://date-fns.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [shadcn/ui](https://ui.shadcn.com/)

## 📝 Environment Variables
```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard
DATABASE_URL=
PIXABAY_API_KEY=
ARCJET_KEY=
```

## 💡 Troubleshooting
- **Hydration errors**: All dates are formatted on the server for consistency.
- **Auth issues**: Double-check Clerk keys and callback URLs.
- **Database errors**: Ensure your DATABASE_URL is correct and migrations are run.

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first.

## 📄 License
[MIT](LICENSE)

---

*Made with ❤️ — Last updated: 2025-04-21*