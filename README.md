# Done With It

A cross-platform mobile marketplace built with React Native and Expo. Features real-time messaging, image uploads, offline support, and geolocation-based listings. Backend powered by Node.js and Express.

[View Portfolio](https://zachayers.io) | [Live Demo](https://expo.dev/@n73311/donewithit)

## About

Done With It is a full-stack mobile application showcasing React Native development with Expo, featuring a Node.js/Express REST API backend. The app allows users to buy and sell items, chat in real-time, and browse listings with offline capabilities.

## Built With

### Mobile App
- React Native
- Expo SDK 40+
- React Navigation
- Formik & Yup (form validation)
- Apisauce (API client)
- Expo Image Picker
- Expo Location
- AsyncStorage

### Backend API
- Node.js 14.x
- Express.js
- Multer (file uploads)
- JWT Authentication
- MongoDB/PostgreSQL

### Tools & Services
- Expo EAS Build
- Cloudinary (image storage)
- Sentry (error tracking)

## Getting Started

### Prerequisites

- Node.js 14.x or higher
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- iOS Simulator (Mac) or Android Studio

### Installation

```bash
git clone https://github.com/n73311/done-with-it.git
cd done-with-it
npm install
```

### Development

Start the Expo development server:

```bash
npm start
```

Run on iOS:

```bash
npm run ios
```

Run on Android:

```bash
npm run android
```

### Backend Setup

The backend API is in a separate repository ([done-with-it-api](https://github.com/n73311/done-with-it-api)). Set the API endpoint in `app/config/settings.js`.

## Features

### Mobile App
- **User Authentication**: JWT-based login and registration
- **Listing Management**: Create, view, and manage item listings
- **Real-Time Messaging**: Chat with buyers/sellers
- **Image Upload**: Multi-image support with Expo Image Picker
- **Geolocation**: Location-based listings and maps
- **Offline Support**: AsyncStorage for offline data persistence
- **Form Validation**: Formik and Yup for robust form handling
- **Error Tracking**: Sentry integration for production monitoring

### Backend API
- **RESTful Endpoints**: Express.js routes for listings, users, messages
- **File Uploads**: Multer middleware for image processing
- **Authentication**: JWT token generation and validation
- **Database**: MongoDB/PostgreSQL for data persistence
- **Image Storage**: Cloudinary integration for scalable image hosting

## Project Structure

```
done-with-it/
├── app/
│   ├── api/           # API client and endpoints
│   ├── auth/          # Authentication context and storage
│   ├── components/    # Reusable UI components
│   ├── config/        # App configuration
│   ├── hooks/         # Custom React hooks
│   ├── navigation/    # React Navigation setup
│   ├── screens/       # App screens
│   └── utility/       # Utility functions
├── assets/           # Images, fonts, and static files
├── App.js           # Entry point
└── app.json         # Expo configuration
```

## Deployment

### Mobile App

Build with EAS Build:

```bash
eas build --platform ios
eas build --platform android
```

Submit to app stores:

```bash
eas submit --platform ios
eas submit --platform android
```

### Backend API

See [done-with-it-api](https://github.com/n73311/done-with-it-api) for deployment instructions.

## License

Licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE) for details.

## Author

Zachariah Ayers - [zachayers.io](https://zachayers.io)
