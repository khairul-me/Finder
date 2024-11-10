# Finder - Campus Marketplace App 🎓

[![Flutter](https://img.shields.io/badge/Built%20with-FlutterFlow-02569B?logo=flutter)](https://flutterflow.io)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Finder is a campus-specific marketplace application that revolutionizes how college communities buy and sell items. Inspired by Tinder's intuitive interface, Finder creates a secure, anonymous platform for students and staff to trade items within their campus community.

## 🎯 Problem Statement

College students often discard useful items during moves or upgrades, while others might need these same items. There's no efficient, campus-specific platform to connect these two groups. Finder bridges this gap while promoting sustainability.

## 🌟 Key Features

- **Campus-Restricted Access**: Secure .edu email verification
- **Tinder-Style Interface**: Intuitive swipe mechanics for browsing items
- **Anonymous Listings**: Privacy-first approach to buying and selling
- **Secure Messaging**: Built-in chat system for buyer-seller communication
- **Smart Categories**: Easy organization of items by type and condition
- **Order Tracking**: Real-time updates on purchase status

## 🔄 System Architecture

### Authentication Flow
```mermaid
flowchart TD
    A[Start] --> B[Splash Screen]
    B --> C[Email Verification]
    C --> D{Valid .edu?}
    D -->|Yes| E[Create/Login Account]
    D -->|No| F[Access Denied]
    E --> G[Role Selection]
    G --> H[Buyer Mode]
    G --> I[Seller Mode]
```

### Seller Flow
```mermaid
flowchart TD
    A[Seller Mode] --> B[Create Listing]
    B --> C[Add Photos]
    C --> D[Item Details]
    D --> E[Set Price]
    E --> F[Preview]
    F --> G[Post Listing]
    G --> H[Active Listings]
    H --> I[Message Center]
    H --> J[Order Management]
```

### Buyer Flow
```mermaid
flowchart TD
    A[Buyer Mode] --> B[Browse Items]
    B --> C[View Details]
    C --> D{Decision}
    D -->|Pass| B
    D -->|Like| E[Shopping Cart]
    D -->|Chat| F[Message Seller]
    E --> G[Payment]
    G --> H[Order Confirmation]
    H --> I[Track Order]
```

### Messaging System
```mermaid
flowchart TD
    A[Message Center] --> B[Inbox]
    B --> C[Chat Threads]
    C --> D[Price Negotiation]
    C --> E[Meeting Arrangement]
    C --> F[Item Questions]
```

## 💻 Technology Stack

- **Frontend**: Flutter/FlutterFlow
- **Backend**: Firebase
- **Authentication**: Firebase Auth
- **Database**: Cloud Firestore
- **Storage**: Firebase Storage
- **Messaging**: Firebase Cloud Messaging

## 🚀 Getting Started

### Prerequisites
- Flutter SDK
- FlutterFlow account
- Firebase project
- Android Studio / VS Code

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/finder-app.git
```

2. Navigate to project directory
```bash
cd finder-app
```

3. Install dependencies
```bash
flutter pub get
```

4. Run the app
```bash
flutter run
```

## 👥 Team

### Core Developers
- **Md Khairul Islam**
  - Institution: Hobart and William Smith Colleges, Geneva, NY
  - Major: Robotics and Computer Science
  - Contact: khairul.islam@hws.edu | (315) 878-9695

- **Md Wasiful Karim**
  - Institution: Ohio Wesleyan University, Ohio, USA
  - Major: Astrophysics and Computer Science
  - Contact: mwkarim@owu.edu | (740) 803-6371

## 📱 App Screenshots

![image](https://github.com/user-attachments/assets/e0dbdf4a-9013-494d-abd7-6e4a2b331190)

## 🤝 Contributing

We welcome contributions to Finder! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- FlutterFlow team for their excellent development platform
- Our college communities for inspiration and support
- All contributors who have helped shape this project

## 📞 Contact

For any queries regarding the application, please contact either of the core developers listed above.

---
Made with ❤️ for College Communities
