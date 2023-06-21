# Quik-a-nik

Quik-a-nik allows users to purchase pre-made picnic baskets or mix and match to create their own, both on web and Android devices using React Native's cross-platform funtionality.

Through our app a user can select any outdoor location for delivery utilizing our Google Maps integration, and pay in advance using the included Stripe payment API.

For more information on who built Quik-a-nik, scroll down to the bottom of the README.md file.

## Screenshots

![Home (Mobile)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Home%20(Mobile).png?raw=true)
![Home (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Home%20(Web).png?raw=true)
![Products List (Mobile)](https://github.com/MorriganH/quik-a-nik/blob/feature/final-style-tweaks/docs/Quik-a-nik%20Products%20(Mobile).png?raw=true)
![Products List (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Products%20(Web).png?raw=true)
![Cart (Mobile)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Cart%20(Mobile).png?raw=true)
![Cart (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Cart%20(Web).png?raw=true)
![Set Location (Mobile)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Set%20Location%20(Mobile).png?raw=true)
![Set Location (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Set%20Location%20(Web).png?raw=true)
![Order Confirmation (Mobile)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Order%20Confirmation%20(Mobile).png?raw=true)
![Order Confirmation (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20Order%20Confirmation%20(Web).png?raw=true)
![My Orders (Web)](https://github.com/MorriganH/quik-a-nik/blob/readme/docs/Quik-a-nik%20My%20Orders%20(Web).png?raw=true)


## Getting Started

- `npm install` in both the frontend and server directories.

- In server, create .env and copy .env.example into it. Ensure `DB_USER` and `DB_PASS` are accurate for your system.  Sign up for a Stripe Developer account and paste your Stripe secret key into the `STRIPE_SECRET` string value.

- In frontend, create api_key.js and copy api_key.js.example into it. Replace `yourKey` with your Google Maps API key.
- In frontend, create stripe_publishable.js and copy stripe_publishable.js.example into it.  Replace `STRIPE_PUBLISHABLE` with your own Stripe Publishable Key from your Stripe Developer account.

### Backend

- `cd server/`
- `npm start`

### Frontend

- `cd frontend/`

#### To run in browser

- `npm run web`

#### To run on Android

- `npx expo start --tunnel`
Download the Expo Go app
Scan the QR code to view your app


#### To allow Android to make axios requests to localhost

Create backend_tunnel.js file within frontend directory and copy backend_tunnel.js.example into it
Global install ngrok using `npm install -g ngrok`.  You will be given an ngrok TOKEN to copy.
Configure ngrok on your system using `ngrok config add-authtoken TOKEN`
Run ngrok with `ngrok http 3000`
Copy the forwarding URL that is generated by ngrok and replace 'NGROK TUNNEL URL HERE' with URL string in backend_tunnel.js file.



### Using The App
Once the app has launched you can do the following:

- Press Login or Register to sign in as a user
- From home screen, press any photo to view all products under a specific category and add them to your basket.
- Press 'Quik-a-nik' in top right corner to be redirected to the home page
- When ready to checkout, press the basket icon in the nav bar to start checkout process.
- Press My Orders to view your past orders made.

### Tech Stack
- React Native
- Express
- PostgreSQL


### Dependencies 

#### Frontend
    "@expo-google-fonts/dm-sans": "^0.2.3",
    "@expo-google-fonts/inter": "^0.2.3",
    "@expo-google-fonts/pacifico": "^0.2.3",
    "@expo/webpack-config": "^18.0.1",
    "@react-google-maps/api": "^2.18.1",
    "@react-navigation/native": "^6.1.6",
    "@react-navigation/native-stack": "^6.9.12",
    "@stripe/react-stripe-js": "^2.1.0",
    "@stripe/stripe-js": "^1.54.0",
    "@stripe/stripe-react-native": "^0.27.2",
    "axios": "^1.4.0",
    "bcryptjs": "^2.4.3",
    "expo": "~48.0.18",
    "expo-device": "~5.2.1",
    "expo-font": "~11.1.1",
    "expo-location": "~15.1.1",
    "expo-status-bar": "~1.4.4",
    "react": "18.2.0",
    "react-dom": "18.2.0",
    "react-native": "0.71.8",
    "react-native-bcrypt": "^2.4.0",
    "react-native-maps": "1.3.2",
    "react-native-safe-area-context": "4.5.0",
    "react-native-screens": "~3.20.0",
    "react-native-svg": "^13.9.0",
    "react-native-web": "~0.18.10",
    "react-native-web-maps": "^0.3.0",
    "react-redux": "^8.0.7",
    "redux": "^4.2.1",
    "redux-thunk": "^2.4.2"

#### Backend
    "body-parser": "^1.20.2",
    "cookie-session": "^2.0.0",
    "cors": "^2.8.5",
    "debug": "~2.6.9",
    "dotenv": "^16.1.4",
    "express": "~4.16.1",
    "morgan": "~1.9.1",
    "ngrok": "*",
    "nodemon": "^2.0.22",
    "pg": "^8.11.0",
    "stripe": "^12.9.0"


### Development Team

#### Graydon Richie
- https://www.linkedin.com/in/graydonritchie/
- https://github.com/SirGraybon

#### Morrigan Hennessey
- https://www.linkedin.com/in/morrigan-hennessy/
- https://github.com/MorriganH

##### Viktor Ristic
- https://www.linkedin.com/in/vikristic/
- https://github.com/vktr-r2

