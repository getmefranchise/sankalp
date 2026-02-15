[README.md](https://github.com/user-attachments/files/25319298/README.md)
# 🕉️ Sadhana - Hindu-Themed Task Management Tool

**साधना** - Transform tasks into sacred practice

[![Firebase](https://img.shields.io/badge/Firebase-Latest-orange)](https://firebase.google.com/)
[![React](https://img.shields.io/badge/React-18-blue)](https://react.dev/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 🌟 Overview

**Sadhana** (साधना) is a comprehensive, Firebase-powered task management application inspired by Hindu philosophy. It combines ancient wisdom with modern technology to help users manage their daily tasks, delegations, and priorities in a spiritually-informed manner.

### Key Features

- ✅ **Pundit-Style Priority System**: Brahma, Vishnu, Shiva, Indra
- 📋 **Advanced Task Management**: Natural language input, subtasks, recurring tasks
- 📅 **Multiple Views**: List, Board, Calendar views (Todoist-inspired)
- 🎯 **Productivity Tools**: Pomodoro timer, habit tracker (TickTick-inspired)
- 👥 **Collaboration**: Task delegation and sharing
- 📊 **Analytics**: Statistics and productivity insights
- 🔐 **Secure Authentication**: Email/password, password reset
- 🌙 **Dark/Light Theme**: Customizable interface
- 📱 **Responsive Design**: Works on all devices
- 🔄 **Real-time Sync**: Instant updates across devices

## 🚀 Quick Start

### Prerequisites

- Node.js 18.x or higher
- npm or yarn
- Firebase account

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/your-username/sadhana-task-manager.git
cd sadhana-task-manager
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up Firebase**
```bash
# Create a Firebase project at https://console.firebase.google.com/
# Copy your Firebase configuration
```

4. **Configure environment variables**
```bash
# Create .env file in project root
cp .env.example .env
# Edit .env with your Firebase configuration
```

5. **Run development server**
```bash
npm run dev
```

6. **Build for production**
```bash
npm run build
```

## 📁 Project Structure

```
sadhana-task-manager/
├── src/
│   ├── components/        # React components
│   │   ├── auth/         # Authentication components
│   │   ├── tasks/        # Task management components
│   │   ├── ui/           # Reusable UI components
│   │   └── layout/       # Layout components
│   ├── firebase/         # Firebase configuration & services
│   ├── contexts/         # React contexts
│   ├── hooks/            # Custom React hooks
│   ├── utils/            # Utility functions
│   └── styles/           # Global styles
├── public/               # Static assets
├── firebase.json         # Firebase configuration
├── package.json
└── README.md
```

## 🔧 Firebase Setup

### 1. Create Firebase Project

- Go to [Firebase Console](https://console.firebase.google.com/)
- Click "Add project"
- Enter project name: `sadhana-task-manager`
- Enable Google Analytics (optional)

### 2. Enable Services

**Authentication**
- Navigate to Authentication
- Enable Email/Password sign-in method

**Firestore Database**
- Navigate to Firestore Database
- Create database
- Choose Test mode initially

**Hosting**
- Navigate to Hosting
- Click "Get Started"

### 3. Get Configuration

- Go to Project Settings
- Scroll to "Your apps" section
- Add web app
- Copy configuration to `.env` file

### 4. Security Rules

Copy the security rules from `FIREBASE_SECURITY_RULES.md` to Firebase Console → Firestore → Rules.

## 📚 Documentation

### Core Documentation Files

- **[PROJECT_SCOPE.md](PROJECT_SCOPE.md)** - Detailed project scope and requirements
- **[MASTER_PROMPT.md](MASTER_PROMPT.md)** - Comprehensive development guide
- **[FIREBASE_SETUP_GUIDE.md](FIREBASE_SETUP_GUIDE.md)** - Firebase configuration instructions
- **[FIREBASE_SECURITY_RULES.md](FIREBASE_SECURITY_RULES.md)** - Database security rules
- **[PROJECT_STRUCTURE.md](PROJECT_STRUCTURE.md)** - Project organization and file structure
- **[DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md)** - Complete deployment instructions

### Key Features Documentation

#### Pundit-Style Priority System

- **Brahma (Highest)**: Red - Critical and urgent tasks
- **Vishnu (High)**: Orange - Important tasks that should be done soon
- **Shiva (Medium)**: Blue - Regular tasks that can be scheduled
- **Indra (Low)**: Green - Tasks that can be done when time permits

#### Task Categories

Default categories include: Work, Personal, Spiritual, Health, Family, Study, Other
- Custom categories can be created by users
- Each category has unique colors and icons

#### Productivity Features

- **Pomodoro Timer**: Built-in focus timer with customizable intervals
- **Habit Tracker**: Track daily habits with streaks
- **Statistics**: Comprehensive task completion analytics
- **Focus Mode**: Distraction-free single-task view

## 🎨 Customization

### Theme Configuration

Edit `src/utils/constants.js` to customize:

```javascript
// Colors
export const COLORS = {
  PRIMARY: '#FF9933',    // Saffron
  SECONDARY: '#4A90E2',  // Blue
  SUCCESS: '#2ECC71',    // Green
  // ... more colors
};

// Priority levels
export const PRIORITY_LEVELS = {
  BRAHMA: { label: 'Brahma', color: '#E74C3C', ... },
  // ... more priorities
};
```

### Firebase Configuration

Edit `.env` file:

```env
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your-project-id
VITE_FIREBASE_STORAGE_BUCKET=your-project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

## 🚢 Deployment

### Deploy to Firebase Hosting

```bash
# Install Firebase CLI
npm install -g firebase-tools

# Login to Firebase
firebase login

# Initialize Firebase
firebase init

# Build application
npm run build

# Deploy
firebase deploy
```

For detailed deployment instructions, see [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md).

## 📖 Usage Guide

### Authentication

1. **Register**: Create an account with email and password
2. **Verify Email**: Check your email for verification link
3. **Login**: Enter your credentials to access the app
4. **Reset Password**: Use "Forgot Password" link if needed

### Task Management

1. **Create Task**: Use the one-line input at the top
2. **Set Details**: Add category, priority, due date
3. **Add Subtasks**: Break down complex tasks
4. **Track Progress**: Update progress percentage
5. **Complete**: Mark task as done when finished

### Productivity Tools

1. **Pomodoro Timer**: Set focus intervals (25 min work, 5 min break)
2. **Habit Tracker**: Create daily habits and track completions
3. **Statistics**: View your productivity trends

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Inspiration**: Inspired by the best features of Todoist and TickTick
- **Philosophy**: Based on Hindu concepts of duty (Dharma/Kartavya)
- **Technology**: Built with React and Firebase
- **Design**: Material-UI for beautiful, accessible components

## 📞 Support

For support, please:
- Open an issue on GitHub
- Check existing documentation
- Review Firebase Console for errors
- Consult the [deployment guide](DEPLOYMENT_GUIDE.md) for common issues

## 🔮 Roadmap

### Planned Features

- [ ] Mobile app (React Native)
- [ ] Calendar integrations (Google, Outlook)
- [ ] Advanced analytics and insights
- [ ] Team collaboration features
- [ ] Voice input for tasks
- [ ] AI-powered task suggestions
- [ ] More habit tracking features
- [ ] Custom themes and backgrounds

### Future Enhancements

- [ ] Offline mode improvements
- [ ] Better accessibility support
- [ ] Performance optimizations
- [ ] More authentication providers
- [ ] Internationalization support

## 📊 Tech Stack

### Frontend
- **React 18** - UI framework
- **Vite** - Build tool
- **React Router** - Routing
- **Material-UI** - UI components
- **Zustand** - State management
- **date-fns** - Date manipulation

### Backend & Database
- **Firebase Auth** - Authentication
- **Cloud Firestore** - Real-time database
- **Firebase Hosting** - Web hosting
- **Firebase Storage** - File storage

### Development Tools
- **ESLint** - Code linting
- **Prettier** - Code formatting
- **Firebase CLI** - Firebase deployment

## 🌐 Links

- **Live Demo**: (Coming soon)
- **Documentation**: [Full Documentation](./docs/)
- **Firebase Console**: [Console](https://console.firebase.google.com/)
- **GitHub Repository**: [Repo](https://github.com/your-username/sadhana-task-manager)

## 📄 License

MIT License - feel free to use this project for personal or commercial purposes.

---

**Made with ❤️ and 🙏 for productivity enthusiasts**

*Sadhana - Transform tasks into sacred practice*
