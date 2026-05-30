# WhishperLock

A privacy-first iOS messenger with end-to-end encrypted chat, voice calls, self-destruct messages, and encrypted file/location sharing — built with SwiftUI and Cloudflare Workers.

## Website & Legal (App Store)

| Page | URL |
|------|-----|
| **App homepage & user guide** | https://aaronyang47.github.io/WhishperLock/ |
| **Privacy Policy** | https://aaronyang47.github.io/WhishperLock/privacy-policy.html |
| **Terms of Service** | https://aaronyang47.github.io/WhishperLock/terms-of-service.html |
| **Support** | https://aaronyang47.github.io/WhishperLock/support.html |
| **Contact** | aaronyang470128@hotmail.com |

Use the Privacy Policy and Support URLs in App Store Connect.

## Project Features

### Backend Features (Cloudflare Worker)
- 🔐 **User Authentication System**
  - User registration, login, logout
  - PBKDF2 password encryption storage
  - JWT Token session management
  - Account deletion functionality
- 💬 **Real-time Chat**
  - WebSocket bidirectional communication
  - Real-time message broadcasting
  - Typing indicator
  - Online users list
- 🗄️ **Data Persistence**
  - Message history storage
  - User profile management
  - Friend relationships
  - Chat room management

### iOS Client Features
- 📱 **Modern UI/UX**
  - SwiftUI native interface
  - Dark mode support
  - Smooth animations
  - Responsive design
- 🔒 **Security**
  - End-to-end encryption
  - Biometric authentication
  - Secure token storage
  - Session management
- 🌐 **Network**
  - WebSocket connection
  - Auto-reconnection
  - Network status monitoring
  - Background state handling

## Technical Stack

### Backend
- Cloudflare Workers
- D1 Database (SQLite)
- WebSocket API
- JWT Authentication

### iOS Client
- SwiftUI
- Combine Framework
- WebSocket
- Keychain Services

## Getting Started

### Prerequisites
- Xcode 15.0+
- iOS 16.0+
- Node.js 18+
- Wrangler CLI

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/WhisperLock.git
cd WhisperLock
```

2. Install backend dependencies
```bash
cd CloudflareWorker
npm install
```

3. Configure environment variables
```bash
cp .env.example .env
# Edit .env with your settings
```

4. Deploy Cloudflare Worker
```bash
npx wrangler deploy
```

5. Open iOS project
```bash
open WhisperLock.xcodeproj
```

6. Build and run in Xcode

## Development

### Backend Development
```bash
# Start local development server
npx wrangler dev

# Run database migrations
npx wrangler d1 migrations apply

# Deploy to production
npx wrangler deploy
```

### iOS Development
1. Open `WhisperLock.xcodeproj` in Xcode
2. Configure signing certificate
3. Select target device/simulator
4. Build and run

## Testing

### Backend Tests
```bash
cd CloudflareWorker
npm test
```

### iOS Tests
Run tests through Xcode's Test Navigator

## Deployment

### Backend Deployment
```bash
cd CloudflareWorker
npx wrangler deploy
```

### iOS App Distribution
1. Configure app signing in Xcode
2. Create archive
3. Upload to App Store Connect

## Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Cloudflare for Workers platform
- Apple for SwiftUI framework
- All contributors and users 