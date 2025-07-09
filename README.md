💬 Simple Chat App (React Native + Firebase)

A real-time Chat Application built using React Native and Firebase. This app allows users to send and receive messages instantly using Firebase’s powerful backend services. It's a clean and minimal chat app designed for learning and demonstration purposes.

🚀 Features

🔐 User authentication (Sign up / Sign in with Firebase Auth)

💬 Real-time one-to-one messaging

🔥 Powered by Firebase Realtime Database or Firestore

🕒 Timestamped messages

🧹 Simple and intuitive UI


🛠️ Tech Stack
React Native

react-native-gifted-chat

react-native-community/google-signin

Firebase (Auth + Firestore)

React Navigation

React Hooks for state and lifecycle management

📦 Installation

bash
Copy
Edit
git clone https://github.com/MahaveerSukhani/Simple_Chat_App.git
cd Simple_Chat_App
npm install
expo start

🔧 Firebase Setup

Create a Firebase project at https://console.firebase.google.com

Follow The Installation at https://github.com/react-native-community/google-signin

Get WebClientID ( Login Page )

Create a Firestore Database

Add your Firebase config in the project:

js
Copy
Edit


* Get WebClientID ( Login Page )

// javascript

GoogleSignin.configure({
   scopes: ["https://www.googleapis.com/auth/userinfo.profile"],
   webClientId: '******', // TODO : Get WebClient ID From Firebase By Enabling Google SIGN In
   offlineAccess: true, // if you want to access Google API on behalf of the user FROM YOUR SERVER
   forceCodeForRefreshToken: true, // [Android] related to `serverAuthCode`, read the docs link below *.
 });


// Firebase Configuration's ( Fire.js )

export const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};


📷 Screenshots

<img src="https://user-images.githubusercontent.com/61349423/94794860-1ab97080-03fa-11eb-8e87-eba1c55b8a4b.jpg" width="282" height="501">

📄 License
This project is licensed under the MIT License.

