# NexusPi

A Swift/SwiftUI iOS app that provides a secure marketplace leveraging Pi Network cryptocurrency for payments and CloudKit for storage.

## Features

- **User Authentication**: Sign in with Apple ID and Pi Network accounts
- **Marketplace**: Buy and sell items using Pi cryptocurrency
- **Secure Storage**: CloudKit integration for data management
- **Real-time Updates**: Live status updates for transactions
- **User Profiles**: Customizable user profiles
- **Search and Filtering**: Find items by category or keyword
- **Modern UI**: Built with SwiftUI for iOS 18+

## Technical Architecture

- **Swift 5.9+**: Modern Swift language features
- **SwiftUI**: Declarative UI framework
- **MVVM Architecture**: Clean separation of concerns
- **CloudKit**: Apple's cloud database service for data storage
- **Pi Network API**: Integration for cryptocurrency transactions
- **Keychain Services**: Secure credential storage
- **Combine Framework**: Reactive programming for data flow

## Project Structure

- **NexusPi/**: iOS app codebase
  - **Models/**: Data models (User, Product, Order)
  - **Views/**: SwiftUI views
  - **ViewModels/**: Business logic
  - **Services/**: API and data services
  - **Utilities/**: Helper functions
- **NexusPi-Web/**: Web components for Pi Network hosting requirements

## Setup Instructions

### Prerequisites

- Xcode 15+
- iOS 18 SDK
- Apple Developer Account
- Pi Network Developer Account

### Development Environment

1. Clone the repository
2. Open NexusPi.xcodeproj in Xcode
3. Configure signing with your Apple Developer account
4. Set up CloudKit containers in Apple Developer portal
5. Add your Pi Network API credentials
6. Build and run on simulator or device

### Web Components

The NexusPi-Web directory contains files needed for Pi Network validation:

1. Host these files on GitHub Pages or another web host
2. Configure your Pi Network developer settings to point to this host
3. Update the URLs in the iOS app to match your hosting setup

## Pi Network Integration

This app is designed to work with the Pi Network cryptocurrency platform:

1. Users authenticate with their Pi Network account
2. The app facilitates transactions using Pi cryptocurrency
3. All transactions are verified through the Pi Network API
4. The app complies with Pi Network's security requirements

## CloudKit Integration

Data is stored and synchronized using Apple's CloudKit:

1. User profiles and preferences 
2. Product listings and details
3. Transaction history
4. User ratings and feedback

## License

This project is for educational purposes. Use responsibly and ensure compliance with:
- Apple's App Store Review Guidelines
- Pi Network Developer Terms of Service 