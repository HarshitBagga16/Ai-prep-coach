
# 🚀 AI Career Coach

An intelligent, full-stack career coaching platform that leverages AI to help users advance their professional journey. Built with Next.js, Prisma, NeonDB, Gemini API, Inngest, Clerk, and Shadcn UI, this app provides personalized guidance, document generation, interview preparation, and real-time industry insights—all in a modern, secure, and scalable web experience.

---

## 🏆 Key Features

- **AI-Powered Onboarding:** Personalized career guidance based on your industry, experience, and skills.
- **Smart Resume Builder:** Create, edit, and export ATS-optimized resumes with markdown and PDF support. Improve sections with AI suggestions.
- **AI Cover Letter Generator:** Instantly generate tailored cover letters for any job using your profile and job description.
- **Mock Interview Prep:** Practice with AI-generated quizzes, get instant feedback, and track your progress over time.
- **Industry Insights Dashboard:** Real-time analytics on salaries, trends, in-demand skills, and market outlook for your field.
- **Secure Auth & User Management:** Powered by Clerk for seamless sign-in, onboarding, and data protection.
- **Modern UI/UX:** Responsive, accessible, and beautiful interface using Shadcn UI and Tailwind CSS.
- **Event-Driven Background Jobs:** Scalable AI tasks and data updates via Inngest workflows.

---

## 🗺️ User Journey

1. **Sign Up & Onboarding:**
   - Register and complete onboarding to personalize your experience.
   - Share your industry, experience, and skills for tailored insights.
2. **Document Creation:**
   - Build your resume with markdown and AI-powered improvements.
   - Generate and manage cover letters for specific jobs.
3. **Interview Preparation:**
   - Take AI-generated quizzes, review answers, and receive improvement tips.
4. **Analytics & Insights:**
   - Access your dashboard for industry trends, salary data, and progress analytics.

---

## 🛠️ Tech Stack

- **Frontend:** Next.js 14, React 19, Tailwind CSS, Shadcn UI
- **Backend:** Prisma ORM, Neon Postgres DB, Inngest (event-driven workflows)
- **AI Integration:** Google Gemini 1.5 Pro (Generative AI)
- **Auth:** Clerk (Authentication & User Management)
- **PDF Export:** html2pdf.js
- **Deployment:** Vercel or any Node-compatible provider

---

## 📂 Project Structure

```
/
├── app/                  # Next.js app directory (routes, pages, API)
├── components/           # Reusable UI components (Shadcn-based)
├── lib/                  # Helpers (Prisma, Inngest, Gemini client setup)
├── actions/              # Server actions and business logic
├── data/                 # Static data (features, industries, FAQs)
├── hooks/                # Custom React hooks
├── prisma/               # Prisma schema and migrations
└── public/               # Static assets (images, icons)
```

---

## 🧪 Detailed Features

- **Onboarding:**
  - Collects user industry, experience, and skills for personalized coaching.
- **Resume Builder:**
  - Form-based and markdown editing, AI improvement, PDF export, and ATS scoring.
- **Cover Letter Generator:**
  - Uses AI to generate professional, job-specific cover letters in markdown.
- **Interview Prep:**
  - AI-powered quizzes with instant scoring, analytics, and improvement tips.
- **Industry Insights:**
  - Real-time salary ranges, growth rates, demand levels, top skills, and trends.
- **Secure Auth:**
  - Clerk-powered sign-in, onboarding, and user session management.
- **Modern UI:**
  - Responsive, accessible, and visually appealing with Shadcn UI and Tailwind.

---

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
# Prisma + NeonDB
DATABASE_URL="your_neon_postgres_url"

# Clerk Auth
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
CLERK_SECRET_KEY="your_clerk_secret_key"

# Clerk URL Config
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

# Gemini AI Key
GEMINI_API_KEY="your_gemini_api_key"
```

---

## 🧑‍💻 Getting Started (Local Setup)

1. **Clone the Repo**

   ```bash
   git clone https://github.com/your-username/ai-career-coach.git
   cd ai-career-coach
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Configure `.env`**
   - Fill in all required keys from Clerk, Neon, and Gemini.

4. **Push Prisma Schema**

   ```bash
   npx prisma db push
   ```

5. **Run the App**

   ```bash
   npm run dev
   ```

6. **(Optional) Lint the Code**

   ```bash
   npm run lint
   ```

---

## 🌐 Deploying to Vercel

1. Connect your repo to Vercel.
2. Add all required `.env` variables in the Vercel dashboard.
3. Deploy and enjoy!

---

## 📜 Scripts

- `npm run dev` – Start the development server
- `npm run build` – Build for production
- `npm run start` – Start the production server
- `npm run lint` – Run ESLint
- `npx prisma db push` – Push schema to database

---

## 📸 Screenshots

| Onboarding Page | AI Quiz Interface |
|-----------------|-------------------|
| ![onboarding](./public/screens/onboarding.png) | ![quiz](./public/screens/quiz.png) |

---

## ✨ Credits

- **UI Kit:** [Shadcn UI](https://ui.shadcn.dev)
- **Events:** [Inngest](https://www.inngest.com/)
- **AI:** [Gemini API](https://ai.google.dev/)
- **Auth:** [Clerk.dev](https://clerk.dev/)
- **DB:** [Neon.tech](https://neon.tech/)
- **ORM:** [Prisma.io](https://prisma.io/)

---

## 📬 Feedback & Contributions

Pull requests and issues are welcome! Help us build the future of AI-powered career coaching.

---

## License

MIT © 2025 – [Harshit Bagga]
