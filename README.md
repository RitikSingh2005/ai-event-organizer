# 🤖 AI Event Organiser

An AI-powered Event Management Platform built with Next.js, Clerk Authentication, and Convex Backend that allows users to create, explore, and manage events intelligently.

Create events in seconds using AI. Manage tickets. Discover events. All in one platform.

# 🚀 Features

🔐 Authentication (Sign In / Sign Up) using Clerk

🤖 AI Event Generation (via /api/generate-event)

🎟️ Event Creation & Management

📍 Location Search & Utilities

🖼️ Unsplash Image Picker Integration

🧾 Ticket Registration System

🌍 Public Event Exploration

🎨 Modern UI with Theme Support

📊 User Dashboard

🔎 Search Functionality

🧠 Onboarding Modal for New Users

# 🏗️ Tech Stack
| Technology               | Usage              |
| ------------------------ | ------------------ |
| **Next.js (App Router)** | Frontend & Routing |
| **Clerk**                | Authentication     |
| **Convex**               | Backend & Database |
| **Tailwind CSS**         | Styling            |
| **Unsplash API**         | Event Images       |
| **AI API**               | Event Generation   |


# 📂 Folder Structure

```bash
ai-event-organizer
│
├── app/                                # Next.js App Router
│   │
│   ├── (auth)/                         # Authentication Routes (Clerk)
│   │   ├── sign-in/[[...sign-in]]/
│   │   └── sign-up/[[...sign-up]]/
│   │   └── layout.js
│   │
│   ├── (main)/                         # Protected Routes (Logged-in Users)
│   │   ├── create-event/
│   │   ├── my-events/
│   │   ├── my-tickets/
│   │   └── layout.js
│   │
│   ├── (public)/                       # Public Routes
│   │   ├── events/
│   │   │   └── [slug]/                 # Dynamic Event Page
│   │   └── explore/
│   │
│   ├── api/                            # API Routes
│   │   └── generate-event/
│   │       └── route.js                # AI Event Generation Logic
│   │
│   ├── layout.js                       # Root Layout
│   ├── page.jsx                        # Landing Page
│   ├── ConvexClientProvider.jsx        # Convex Provider
│   ├── globals.css
│   └── favicon.ico
│
├── components/                         # Reusable UI Components
│   │
│   ├── ui/                             # ShadCN / UI primitives
│   │
│   ├── event-card.jsx
│   ├── header.jsx
│   ├── onboarding-modal.jsx
│   ├── search-location-bar.jsx
│   ├── theme-provider.jsx
│   ├── unsplash-image-picker.jsx
│   └── upgrade-modal.jsx
│
├── convex/                             # Convex Backend
│   │
│   ├── _generated/                     # Auto-generated Convex files
│   │
│   ├── auth.config.js                  # Clerk + Convex auth config
│   ├── schema.js                       # Database Schema
│   ├── events.js                       # Event CRUD operations
│   ├── registrations.js                # Ticket Registration Logic
│   ├── users.js                        # User management
│   ├── search.js                       # Search functionality
│   ├── dashboard.js                    # Dashboard analytics
│   └── seed.js                         # Seed data
│
├── hooks/                              # Custom React Hooks
│   ├── use-convex-query.jsx
│   ├── use-onboarding.jsx
│   └── use-store-user.js
│
├── lib/                                # Utility & Helper Functions
│   ├── data.js
│   ├── location-utils.js
│   └── utils.js
│
├── public/                             # Static Assets
│   ├── hero.png
│   ├── hero.gif
│   ├── spott.png
│   └── 3d-react.png
│
├── .gitignore
├── README.md
├── components.json                     # ShadCN config
├── eslint.config.mjs
├── jsconfig.json
├── next.config.mjs
├── postcss.config.mjs
├── proxy.js
├── package.json
└── package-lock.json
```
# ⚙️ Installation
### 1️⃣ Clone the repository
git clone https://github.com/your-username/ai-event-organiser.git
cd ai-event-organiser
### 2️⃣ Install dependencies
npm install
### 3️⃣ Setup Environment Variables
###### Create a .env.local file:
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
CONVEX_DEPLOYMENT=
NEXT_PUBLIC_CONVEX_URL=
OPENAI_API_KEY=
UNSPLASH_ACCESS_KEY=

# 📸 Screenshot
![Image Alt](https://github.com/RitikSingh2005/ai-event-organizer/blob/main/Screenshot%202026-03-01%20001404.png)

# 👨‍💻 Author

Ritik Singh

