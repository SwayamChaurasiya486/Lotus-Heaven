# 🌸 Bloom Haven BnB (Lotus Heaven)

An enterprise-grade, full-stack Boutique Bed & Breakfast booking and guest experience management application. Built using a modern monorepo architecture with a **React + TypeScript** frontend and a **NestJS + Prisma** backend, this application provides users with interactive booking, real-time messaging, AI integrations, 3D property maps, and comprehensive administrative controls.

---

## 🚀 Features

### 🏨 Guest Experience & Booking
* **Interactive Booking Flow:** Seamless step-by-step reservation wizard with real-time room availability checks.
* **3D Property Explorer:** Interact with a virtual 3D room tour and floor blueprint viewer using Three.js / React Three Fiber.
* **Smart Search:** Enhanced search and filtering by price, amenities, date ranges, and guest capacities.
* **Weather Intelligence:** Contextual weather widgets suggesting guest experiences based on real-time forecast data.
* **Room Comparison:** Side-by-side amenity and price comparison tool.
* **Travel Memories & Itineraries:** Share trip journals, map out custom travel itineraries, and track vacation expenses.

### 🤖 AI & Real-time Integrations
* **AI Image Generator:** Synthesizes custom scenery images for destinations.
* **AI Recommendations:** Localized, context-aware suggestions for stays and activities.
* **Live Chat & Voice Assistant:** Instant floating messaging widget for guest queries and voice commands.
* **Real-time Notifications:** Toast-based notifications for bookings, reviews, and updates powered by WebSockets.

### 🛡️ Administration & Security
* **Admin Dashboard:** High-level performance tracking, booking analytics, guest listings, and interactive availability calendars.
* **Secure Authentication:** JWT token authentication stored securely using `HttpOnly` and `SameSite` cookies with refresh rotation.
* **Payment Integration:** Multi-processor checkout workflow supporting **Stripe** and **Razorpay**.
* **Mutating Audit Logs:** Interceptor-level tracking of database alterations for full transparency.

---

## 🛠️ Tech Stack

### Frontend
* **Core:** React 18, TypeScript, Vite
* **Routing:** React Router DOM
* **State & Query:** Zustand, TanStack React Query (Axios)
* **Styling:** Tailwind CSS, Shadcn/ui, Framer Motion
* **Visuals:** Three.js / React Three Fiber (R3F)

### Backend
* **Core:** NestJS (Node.js framework), TypeScript
* **Database & ORM:** Prisma ORM, PostgreSQL (Neon Server in production)
* **Caching & Queue:** Redis, BullMQ
* **Security:** Passport JWT, Cookie Parser, Bcrypt
* **Utilities:** Swagger API Docs, Winston (Nest Logger), Resend (Transactional Email)

---

## 📂 Project Structure

```
├── .github/workflows/       # GitHub Actions CI/CD pipeline
├── backend/                 # NestJS App Directory
│   ├── prisma/              # Schema definition & migrations
│   ├── src/                 # Backend TypeScript source code
│   └── Dockerfile           # Production Docker configuration
├── public/                  # Static assets & service workers
├── src/                     # React App Directory
│   ├── components/          # Reusable UI & custom features
│   ├── hooks/               # Custom React hooks (AI, voice, state)
│   ├── lib/                 # Global stores, API clients & styling
│   └── pages/               # Routing views (Dashboards, Room Detail, Travel journal)
├── docker-compose.yml       # Production-like multi-container orchestrator
└── package.json             # Root frontend configuration
```

