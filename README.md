🔐 React Native Password Generator

A simple React Native mobile application that generates secure random passwords based on user preferences.

Users can choose:

Password length

Lowercase letters

Uppercase letters

Numbers

Symbols

The application uses Formik for form handling and Yup for validation.

📱 Features

Generate secure random passwords

Custom password length (4–16 characters)

Toggle character types

Input validation with Yup

Interactive checkboxes using react-native-bouncy-checkbox

Long press to copy generated password

Clean mobile UI

🛠️ Technologies Used

React Native

TypeScript

Formik

Yup

React Native Bouncy Checkbox

📂 Project Structure
password-generator
│
├── src
│   └── App.tsx
│
├── android
├── ios
├── index.js
├── package.json
└── README.md
⚙️ Installation

Clone the repository:

git clone https://github.com/your-username/password-generator.git

Navigate to the project directory:

cd password-generator

Install dependencies:

npm install
▶️ Running the Project

Start Metro bundler:

npm start

Run on Android:

npx react-native run-android

Run on iOS:

npx react-native run-ios
🧠 How It Works

User enters a password length.

User selects character types.

The application builds a list of allowed characters.

Random characters are selected from this list.

A secure password is generated and displayed.

🔑 Password Generation Logic

The password is created by selecting random characters from the selected character set.

Example logic:

const characters = lowercase + uppercase + numbers + symbols

Random character selection:

const index = Math.floor(Math.random() * characters.length)

This process repeats for the chosen password length.

🚀 Future Improvements

Copy button for password

Password strength meter

Dark mode support

Animated UI

Password history

👨‍💻 Author

Developed as a React Native learning project.
