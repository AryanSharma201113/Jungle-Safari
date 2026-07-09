🚀 Multi-Tenant SaaS Architecture
Dynamic Branding & Themes: Operators register through an onboarding portal. Once onboarded, the system fetches their brand settings (logos, address, and unique theme color keys) and dynamically injects them into the UI using CSS Custom Properties (--primary-color, --primary-hover).
Unified Routing: Clean, semantic URL slug matching /corbett-trails/booking maps seamlessly to dynamic configurations, allowing hundreds of custom booking channels on a single codebase.
🧠 Google Gemini AI Integrations
🔥 Immersive Campfire Narrator (AiCampfire.jsx): Crafts rich, atmospheric, suspenseful stories of Kumaon forest legends. Synthesizes an interactive audio stream using the Web Speech API, with automatic regex-based sound-effect filter cleanups and custom speed configurations.
🗺️ Dynamic Jungle Itinerary Planner (JunglePlanner.jsx): Analyzes group dynamics, visit duration, and personal interests to curate the ultimate day-by-day expedition layout.
📊 Sighting Probability Predictor (Sightings.jsx): Uses advanced logic models calibrated for seasonal trends, weather patterns, and regional animal frequencies to forecast real-time sighting metrics.
👁️ Wildlife Vision Scanner (ChatBot.jsx): Uses Gemini Vision capabilities to instantly scan safari photos, identifying species and providing detailed ecological details.
💬 Natural Conversational Booking Agent (ChatBot.jsx): Guides guests in planning their ride by extracting booking parameters organically from a standard chat conversation.
✉️ Resilient Dual-Channel Dispatcher
High Availability: Features a failover mail pipeline that leverages SendGrid as the primary dispatcher and Nodemailer as an automatic fallback, complete with local sandbox previews.
📁 Repository Directory Structure
JungleSafari/
├── backend/                   # Node.js + Express API Gateway
│   ├── controllers/           # Request handlers & logic
│   ├── middlewares/           # JWT authentications & common utilities
│   ├── models/                # MongoDB (Mongoose) dynamic schemas
│   ├── routes/                # Endpoint mapping (AI, Tenants, Bookings)
│   ├── utils/                 # Gemini API client, auto-admin, & mailers
│   └── package.json           # Backend dependencies
│
└── frontend/                  # React + Vite Client Application
    ├── public/                # Static assets & icons
    ├── src/
    │   ├── components/        # Dynamic Header, Chatbot, & Home blocks
    │   ├── pages/             # Booking forms, AI Campfire, Live Sightings
    │   ├── App.jsx            # Multi-Tenant routing dispatcher
    │   ├── index.css          # Design system stylesheet
    │   └── main.jsx           # Client mounting
    └── package.json           # Frontend packages
    
