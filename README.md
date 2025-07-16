📚 LMS SaaS App – Full-Stack Learning Platform
A modern, scalable Learning Management System (LMS) SaaS application built from scratch using Next.js, Supabase, Clerk, Stripe, and Vapi. This platform empowers users to create, manage, and interact with AI voice tutors—enhancing the online learning experience with real-time conversation, personalized content, and robust session tracking.

🚀 Live Preview
Coming soon (Add your deployed link here if available)

🔋 Features (Detailed)
🎙️ AI Voice Tutors
Create intelligent, voice-powered AI tutors that interact with users in real-time. Powered by Vapi, these tutors use speech-to-text and text-to-speech engines to:

Respond to students in a human-like voice

Adapt to different teaching styles (e.g., formal, friendly)

Stick to assigned topics and subjects

Conduct interactive tutoring sessions

🔐 User Authentication
Secure login and user management using Clerk, with support for:

Email and password registration

OAuth (e.g., Google) login

Session handling and protected routes

Conditional UI based on authentication state

💳 Subscription & Billing
Handle user plans and access control using Stripe, including:

Free and premium tiers

Monthly/annual plans

Payment checkout, cancellation, and upgrade flows

Feature locking based on plan (e.g., number of tutors a user can create)

🧠 Create Your Own Tutor
Users can generate custom AI tutors by selecting:

Subject (e.g., Math, Physics)

Topic (e.g., Algebra, Thermodynamics)

Conversation Style (e.g., formal, enthusiastic)

This feature helps learners get tailored experiences from the voice tutor based on their needs.

⭐ Bookmarking
Allow users to bookmark their favorite tutors so they can easily find and access them later. Bookmarked tutors are stored in the database and can be accessed across devices.

🧾 Session History
Every AI conversation is stored with metadata like:

Date and time of session

Tutor used

Duration

Users can revisit old sessions, review concepts, or track their learning progress.

🔍 Smart Search & Filters
Help users discover the right tutor using:

Subject-based filtering

Keyword matching on tutor name or topic

Dynamic filtering UI

Enables faster and more intuitive navigation through large sets of tutors.

📱 Fully Responsive Design
The entire app is designed using Tailwind CSS and shadcn/ui, ensuring:

Mobile-first layout

Tablet and desktop support

Seamless transitions and responsive breakpoints

🛠️ Modular Code & Reusability
Clean folder structure and reusable components:

Scalable for future features

Easy to maintain and extend

Encourages collaboration

🧾 Usage Limits & Role Management
Based on subscription plans, the app enforces:

Tutor creation limits

Feature accessibility (e.g., access to history/bookmarks)

Pro-only features

Useful for building a real-world SaaS with tiered access.

📊 Error Monitoring
Integrated with Sentry for:

Real-time error tracking

Stack trace analysis

Debugging production issues efficiently



🛠 Tech Stack
Tech	Purpose
Next.js	React framework for full-stack features like SSR and API routes
Supabase	Backend-as-a-service for real-time DB, auth, and storage
Clerk	User authentication and access control
Stripe	Secure payments and subscription billing
Vapi	Low-latency AI voice agent for tutor interaction
Tailwind CSS	Utility-first CSS for responsive UI
shadcn/ui	Pre-built accessible components with Radix UI
TypeScript	Type safety and better tooling
Zod	Schema validation for backend and forms
Sentry	Monitoring and real-time error reporting

💡 Use Cases
Students looking to learn interactively with AI voice support.

Tutoring platforms wanting to automate sessions.

EdTech startups needing a scalable, full-stack LMS base.

Developers building subscription-based platforms with voice AI integration.

📂 Project Structure
php
Copy
Edit
├── app/                 # Application routes and pages
├── components/          # Reusable UI components
├── lib/                 # Utilities, Supabase, Clerk, Vapi clients
├── public/              # Static assets
├── types/               # Global TypeScript types
├── constants/           # Static config like voices and subject colors
└── styles/              # Global styles (Tailwind)
🧪 Local Setup
Prerequisites
Node.js ≥ 18

npm or yarn

Supabase & Clerk accounts

Steps
bash
Copy
Edit
# Clone repo
git clone https://github.com/your-username/lms-saas-app.git
cd lms-saas-app

# Install dependencies
npm install

# Add environment variables
cp .env.local.example .env.local
# Then fill in:
# - NEXT_PUBLIC_SUPABASE_URL
# - NEXT_PUBLIC_SUPABASE_ANON_KEY
# - CLERK_SECRET_KEY
# - STRIPE_SECRET_KEY
# - NEXT_PUBLIC_VAPI_WEB_TOKEN
# ...etc.

# Start development server
npm run dev
Visit http://localhost:3000 to view the app.

📌 TODOs & Improvements
 Add tutor rating & feedback system

 Enable real-time collaboration sessions

 Add dashboard analytics for users and admins

 Deploy to Vercel (or your preferred platform)

📬 Feedback
I’m open to contributions and suggestions. If you found this project helpful or inspiring, feel free to ⭐ the repo or reach out!
