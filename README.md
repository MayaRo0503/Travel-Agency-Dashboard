# Tourvisto
<!-- Tech Stack Badges -->
<p align="center">
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white" />
  <img alt="React Router" src="https://img.shields.io/badge/React%20Router-v7.0.0-CA4245?style=for-the-badge&logo=react-router&logoColor=white" />
  <img alt="Vite" src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
  <img alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img alt="Syncfusion" src="https://img.shields.io/badge/Syncfusion-0078D4?style=for-the-badge&logo=syncfusion&logoColor=white" />
  <img alt="Appwrite" src="https://img.shields.io/badge/Appwrite-000000?style=for-the-badge&logo=appwrite&logoColor=white" />
  <img alt="Sentry" src="https://img.shields.io/badge/Sentry-000000?style=for-the-badge&logo=sentry&logoColor=white" />
  <img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-000000?style=for-the-badge&logo=openai&logoColor=white" />
</p>

Tourvisto is a dynamic travel dashboard application built with **React** (using React Router v7) and **Tailwind CSS**. It provides personalized travel suggestions, interactive charts and tables, and a powerful admin interface to manage travel data and user information. Whether you're an avid traveler looking for trip ideas or a travel agency managing client itineraries, Tourvisto offers a sleek, modern platform to visualize insights and streamline travel planning. *(Note: This project is currently under development and not deployed live.)*

## ✨ Features

- **Personalized Travel Suggestions:** Get customized destination and itinerary recommendations based on user preferences and past trips.
- **Interactive Charts & Analytics:** Visualize travel data with rich **charts** and **graphs** (powered by Syncfusion) for insights like upcoming trips, budget usage, and travel stats.
- **Admin Dashboard & User Management:** Secure admin panel to manage users and trips. View all registered users in dynamic tables, analyze user activity, and maintain travel records.
- **Trip Management & Forms:** Add new trips with a dedicated form, including fields for destinations, dates, and more. An **AI-powered trip planner** assists in generating itinerary details automatically.
- **Detailed Trip View:** Drill down into each trip to see all details at a glance, including travel dates, destinations, activities, and suggestions. Easily monitor and update trip information.
- **Authentication & Security:** User authentication is handled via Appwrite, ensuring secure login/signup and protected routes for admin features. Error tracking is integrated with Sentry for monitoring and debugging.

## 🚀 Getting Started

Follow these steps to run **Tourvisto** locally on your machine.

### Prerequisites
- **Node.js** and **npm** (or **Yarn**) installed.
- An Appwrite instance (or account) if you want to enable backend features like authentication. *(Alternatively, you can adjust the code to use your own backend or skip if exploring frontend-only.)*

### Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MayaRo0503/Travel-Agency-Dashboard.git
   ```
   Then navigate into the project directory:
   ```bash
   cd Travel-Agency-Dashboard
   ```

2. **Install dependencies:** Use npm or yarn to install the required packages.
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure environment:**

Before running the app, create a `.env.local` (or `.env`) file in your project root and add your own keys for each service. For example:

```dotenv
# Syncfusion license key
VITE_SYNCFUSION_LICENSE_KEY=your_syncfusion_license_key_here

# Appwrite (backend) configuration
VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id_here
VITE_APPWRITE_API_KEY=your_appwrite_api_key_here
VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id_here
VITE_APPWRITE_USERS_COLLECTION_ID=your_appwrite_users_collection_id_here
VITE_APPWRITE_TRIPS_COLLECTION_ID=your_appwrite_trips_collection_id_here
VITE_APPWRITE_API_ENDPOINT=https://your-appwrite-endpoint/v1

# Gemini (AI) API key
GEMINI_API_KEY=your_gemini_api_key_here

# Unsplash (image) API key
UNSPLASH_ACCESS_KEY=your_unsplash_access_key_here
```

4. **Start the development server:** 
   ```bash
   npm run dev
   ```
   *If using Yarn, run `yarn dev`. If your setup is from Create React App (not Vite), use `npm start` instead.* This will launch Tourvisto at `http://localhost:3000` (or another port, as specified in your console). You should see the dashboard in your browser once the server is running.

5. **Build for production (optional):**
   ```bash
   npm run build
   ```
   This will create an optimized production build of the app in the `build` or `dist` directory, ready for deployment.
## 📸 Screenshots

- **Sign-In Page:**  
  ![Sign-In Page](https://i.postimg.cc/MZFjjgGk/sign-in-page.png)

- **Admin Dashboard (Overview):**  
  ![Admin Dashboard Overview](https://i.postimg.cc/SsZYdv7M/dashboard-admin.png)

- **Admin Dashboard (Statistics):**  
  ![Admin Dashboard Statistics](https://i.postimg.cc/bJY2QhbP/dashboard-down-admin.png)

- **All Users Page:**  
  ![All Users Page](https://i.postimg.cc/1zQF363f/all-users-page.png)

- **All Trips Page:**  
  ![All Trips Page](https://i.postimg.cc/02KKGZ6z/trips-page.png)

- **Create Trip Page:**  
  ![Create Trip Page](https://i.postimg.cc/DzPXJZS5/create-trip-page.png)

- **Trip Detail Page (Overview):**  
  ![Trip Detail Overview](https://i.postimg.cc/SRJ2vfDt/trip-detail-page.png)

- **Trip Detail Page (Itinerary):**  
  ![Trip Detail Itinerary](https://i.postimg.cc/1X2nhVdR/trip-detail-down-page.png)

## 🛠 Tech Stack

Tourvisto is built with a modern web development stack and libraries:

- **React** & **React Router v7** – Core UI library and declarative routing for single-page application navigation.
- **Vite** – Blazing-fast development build tool and dev server for React.
- **Tailwind CSS** – Utility-first CSS framework for rapidly building custom designs.
- **Syncfusion React UI** – Suite of pre-built components used for charts, graphs, and other rich visualizations in the dashboard.
- **Appwrite** – Open-source backend-as-a-service for authentication, database, and storage (providing the app's backend API and user management).
- **Sentry** – Real-time error tracking and monitoring tool integrated to catch and report application errors.
- **AI Integration** – (e.g., OpenAI API) Used to power the intelligent trip itinerary generation feature.
- **JavaScript (ES6+)** – The primary programming language for React and frontend logic.

## 🏛️ Architecture

The project is organized to separate backend integrations, routing logic, UI components and static assets:

```plaintext
TRAVEL-AGENCY
├── app
│   ├── appwrite
│   │   ├── auth.ts
│   │   ├── client.ts
│   │   ├── dashboard.ts
│   │   └── trips.ts
│   ├── constants
│   │   ├── index.ts
│   │   └── world_map.ts
│   ├── lib
│   │   └── utils.ts
│   └── routes
│       ├── admin
│       │   ├── admin-layout.tsx
│       │   ├── all-users.tsx
│       │   ├── create-trip.tsx
│       │   ├── dashboard.tsx
│       │   ├── trip-detail.tsx
│       │   └── trips.tsx
│       ├── api
│       │   └── create-trip.ts
│       └── root
│           ├── page-layout.tsx
│           ├── sign-in.tsx
│           └── travel-page.tsx
├── components
│   ├── Header.tsx
│   ├── index.ts
│   ├── InfoPill.tsx
│   ├── MobileSideBar.tsx
│   ├── NavItems.tsx
│   ├── StatsCard.tsx
│   └── TripCard.tsx
├── public
│   └── assets
│       ├── icons
│       ├── images
│       └── photos
├── .dockerignore
├── .env.local
├── .gitignore
├── Dockerfile
├── instrument.server.js
├── package-lock.json
├── package.json
├── react-router.config.ts
├── README.md
├── travel-agency.code-workspace
├── tsconfig.json
└── vite.config.ts
```

## 🙏 Credits

This project was inspired by and developed with guidance from the following resources:

- **JavaScript Mastery Tutorial:** [Build and Deploy a Full Stack React Admin Dashboard for a Travel Agency](https://www.youtube.com/watch?v=xZ1ba-RLrjo) – *A comprehensive YouTube tutorial that formed the foundation of this project.*
- **JavaScript Mastery Pro Upgrade Kit:** [Tourvisto Upgrade Kit](https://jsm.dev/tourvisto-upgrade) – *An extended resource providing additional features and enhancements (such as AI integration and advanced components) for the project.*

Special thanks to the **JavaScript Mastery** team for the excellent tutorial and resources that made this project possible. Happy traveling! 🌍✈️
