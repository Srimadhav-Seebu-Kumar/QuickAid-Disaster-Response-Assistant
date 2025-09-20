# QuickAid - Disaster Response Assistant

![QuickAid Banner](https://via.placeholder.com/800x200/1e40af/ffffff?text=QuickAid+Disaster+Response+Assistant)

## 🚨 Project Vision

QuickAid is an offline-first Progressive Web Application (PWA) designed to be a critical lifeline during disasters and emergencies. When infrastructure fails and internet connectivity becomes unreliable, QuickAid continues to function, providing essential information about nearby hospitals, emergency shelters, and critical resources. Our vision is to create a resilient, accessible tool that works across all devices - from smartphones to feature phones via SMS - ensuring no one is left without vital emergency information when they need it most.

## ✨ Key Features

### 🌐 Offline-First Architecture
- **Service Worker Technology**: Complete functionality without internet connection
- **Local Data Storage**: Critical emergency data cached locally
- **Progressive Enhancement**: Automatically syncs when connection is restored

### 🏥 Emergency Resource Locator
- **Hospital Finder**: Locate nearest hospitals with real-time capacity data
- **Shelter Mapping**: Emergency shelters, evacuation centers, and safe zones
- **Essential Services**: Pharmacies, food banks, and emergency services
- **Resource Status**: Live updates on availability and capacity

### 🛣️ Smart Routing & Navigation
- **Hazard-Aware Routing**: Routes that avoid flood zones, damaged roads, and danger areas
- **Multi-Modal Navigation**: Walking, driving, and public transport options
- **Offline Maps**: Pre-downloaded regional maps for navigation without internet
- **Real-Time Updates**: Traffic and hazard information when connectivity allows

### 📱 Universal Accessibility
- **Progressive Web App**: Works on all modern browsers and devices
- **SMS Gateway Integration**: Critical features accessible via SMS for feature phones
- **Multilingual Support**: Local language support for diverse communities
- **Voice Navigation**: Audio guidance for visually impaired users
- **Low-Bandwidth Mode**: Optimized for poor network conditions

### 🔄 Real-Time Communication
- **Emergency Broadcasts**: Receive official emergency alerts and updates
- **Community Reports**: Crowdsourced hazard and resource information
- **Family Safety**: Check-in features for family coordination
- **Emergency Contacts**: Quick access to local emergency services

## 📁 Project Structure

```
QuickAid-Disaster-Response-Assistant/
├── backend/
│   ├── api/
│   │   ├── routes/
│   │   ├── middleware/
│   │   └── controllers/
│   ├── services/
│   │   ├── sms-gateway/
│   │   ├── geolocation/
│   │   └── emergency-data/
│   ├── database/
│   │   ├── migrations/
│   │   └── models/
│   └── config/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── utils/
│   ├── public/
│   │   ├── manifest.json
│   │   ├── service-worker.js
│   │   └── offline-maps/
│   └── assets/
├── data/
│   ├── emergency-contacts/
│   ├── hospitals/
│   ├── shelters/
│   └── hazard-zones/
└── docs/
    ├── api/
    ├── deployment/
    └── user-guides/
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- MongoDB (for backend data storage)
- Redis (for caching and real-time features)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Srimadhav-Seebu-Kumar/QuickAid-Disaster-Response-Assistant.git
   cd QuickAid-Disaster-Response-Assistant
   ```

2. **Install dependencies**
   ```bash
   # Install backend dependencies
   cd backend
   npm install
   
   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. **Environment Setup**
   ```bash
   # Copy environment templates
   cp backend/.env.example backend/.env
   cp frontend/.env.example frontend/.env
   
   # Configure your environment variables
   # Add your MongoDB connection string, SMS API keys, mapping service keys, etc.
   ```

4. **Database Setup**
   ```bash
   cd backend
   npm run db:migrate
   npm run db:seed
   ```

5. **Start Development Servers**
   ```bash
   # Terminal 1: Start backend server
   cd backend
   npm run dev
   
   # Terminal 2: Start frontend development server
   cd frontend
   npm start
   ```

6. **Access the Application**
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:8000`

## 🏗️ Build for Production

```bash
# Build frontend for production
cd frontend
npm run build

# Build and optimize service worker
npm run build:sw

# Build backend
cd ../backend
npm run build

# Start production server
npm run start:prod
```

## 🧪 Testing

```bash
# Run all tests
npm run test

# Run frontend tests
cd frontend
npm run test

# Run backend tests
cd backend
npm run test

# Run offline functionality tests
npm run test:offline
```

## 📱 PWA Features

- **Installable**: Can be installed on home screen like a native app
- **Offline Capable**: Full functionality without internet connection
- **Push Notifications**: Emergency alerts and updates
- **Background Sync**: Updates data when connection is restored
- **Responsive Design**: Works on all screen sizes

## 🌍 Contributing

We welcome contributions from the community! This project can save lives, and every contribution matters.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

See our [Contributing Guide](docs/CONTRIBUTING.md) for more details.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Emergency Contacts

If you're experiencing a real emergency, please contact your local emergency services immediately:
- US: 911
- EU: 112
- UK: 999
- India: 100/108

This application is designed to complement, not replace, official emergency services.

## 🙏 Acknowledgments

- Emergency services and first responders worldwide
- Open source mapping and geolocation services
- The disaster preparedness and response community
- Contributors and maintainers of this project

---

**Remember: In a real emergency, always contact your local emergency services first. QuickAid is designed to provide additional support and information during crisis situations.**
