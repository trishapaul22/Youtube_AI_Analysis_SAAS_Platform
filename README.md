🚀 HowToYT — AI YouTube Content Assistant
📌 Overview

HowToYT is an AI-powered web application built with Next.js that helps YouTube creators generate content ideas, create thumbnails, analyze trends, and optimize video planning using AI tools.

The platform combines AI automation, modern UI, authentication, and subscription management to provide an all-in-one creator assistant.

✨ Features
🎬 AI Content Generator – Generate video ideas, titles, and scripts.
🖼️ AI Thumbnail Generator – Create thumbnails using AI prompts.
🔍 Thumbnail Search – Analyze competitor thumbnails.
📈 Trending Keywords – Discover trending YouTube topics.
👤 User Dashboard – Central hub for all tools.
🔐 Authentication System – Secure user login & protected routes.
💳 Billing & Subscription – Manage plans and access.
⚙️ Background Jobs – Async processing using Inngest.
🧱 Tech Stack

Frontend

Next.js (App Router)
React
Tailwind CSS
ShadCN UI

Backend

Next.js API Routes
Server Actions

Database

Drizzle ORM + SQL Database

Other Services

AI APIs
Inngest (event workflows)
📂 Project Structure
app/
 ├── (auth)/              # Authentication pages
 ├── (routes)/            # Main features
 │    ├── dashboard
 │    ├── ai-content-generator
 │    ├── ai-thumbnail-generator
 │    ├── trending-keywords
 │    ├── thumbnail-search
 │    ├── billing
 │    └── profile
 ├── api/                 # Backend APIs
 ├── layout.tsx
 └── provider.tsx

components/               # Reusable UI
lib/                      # Utilities
services/                 # Business logic
drizzle/                  # Database schema
middleware.tsx            # Route protection
⚙️ Workflow
User logs in → Authentication verified via middleware.
User enters Dashboard.
Selects an AI tool.
Request sent to backend API.
AI service processes input.
Results returned and displayed.
Data optionally stored in database.
Login → Dashboard → Select Feature → API → AI Processing → Result
🔐 Authentication
Middleware protects private routes.
Unauthenticated users are redirected to login.
Sessions control feature access.

🗄️ Database Usage
Stores:
User information
Generated content
Subscription details
Usage data

Managed using Drizzle ORM.

▶️ Getting Started
Install dependencies
npm install
Run development server
npm run dev

Open:

http://localhost:3000
🌟 Key Highlights
Modern Next.js App Router architecture
AI-powered creator tools
Secure authentication & billing
Scalable API-based backend
Clean component-based UI
