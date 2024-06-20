Steps to Set Up and Deploy the GuessTheFlagMultiplayer App Using Firebase
1.	Create a Firebase Project
    + Visit the [Firebase Console](https://console.firebase.google.com/)
    ![CreateAProject1](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/b386ca11-1f0a-4666-9e77-1852cfb7228b)
    + Click on “Create a project” and follow the prompts to name your project.
    ![CreateAProject2](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/a9e50a82-8a19-47e0-9b5e-c695bf1f0d43)
    + Optionally, enable Google Analytics for your project.
    ![CreateAProject3](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/d3d04bf5-cde1-4d7a-8f21-e1abae91a20c)
    + Click “Create project” and wait for the process to complete.
    ![CreateAProject4](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/9f97d4b6-90b5-43fb-b03e-7739cfa03599)
2.	Enable Firebase Products
    + Navigate to the “Build” category in your project dashboard.
    + Enable the following products:
        + Authentication
        + Firestore Database
        + Hosting
        ![ChooseProducts](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/0a30f97b-c955-459e-b912-45832fd64931)
    + Go to the Authentication tab and click on "Get started".
    ![Authentication1](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/80627a8c-fa78-43af-b54c-36f0ac464cd4)
    + Select the Sign-in method tab.
    ![Authentication2](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/3b29b805-6e52-4b3f-8f6b-f5452a4eb2c1)
    + Enable the Email/Password sign-in method and press "Save".
    ![Authentication3](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/541b51c9-9413-42a6-b293-33b7ec98dfd5)
    ![Authentication4](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/8ed084b2-404c-4b38-b8d9-387f883780f2)
4.	Set Up Firestore Database
    + Go to the Firestore Database tab and click on “Create database.”
    ![Firestore1](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/118536fd-a1fd-43ed-8ec3-5ebb94f0932d)
    + Select a location.
    ![Firestore2](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/4aa9ffe7-14a3-4e77-8888-e53eacc10f4f)
    + Choose to start in test mode and proceed with the setup.
    ![Firestore3](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/6aab8cc5-3e0c-4580-8664-aa4b42d6baff)
    + Your database should be empty.
    + The database automatically fills itself with data as soon as the website is accessed.
    ![Firestore4](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/82c3d0a1-3858-4f20-9283-45f19e025f46)
5.	Add a Web App to Your Project
    + In the Project Overview, click on the “Add app” button and select the web icon (“</>”).
    ![AddWebApp1](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/79a78736-e00d-4116-8aff-c2d50733a494)
    + Give your web app a nickname and register it.
    ![AddWebApp2](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/b2fa2fcf-6348-46c6-ba5a-2f44f4070485)
    + Copy the provided firebaseConfig object.
    ![AddWebApp3](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/c6f7a1a8-ca80-4bc8-bcb7-f23c8af14074)
6.	Download and Set Up the GuessTheFlagMultiplayer App
    + Download the latest release zip from [GitHub](https://github.com/if23b011/GuessTheFlagMultiplayer/releases/latest)
    ![DownloadZIP](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/df6e1c28-8d3b-4ae2-a59c-6411b5d7e3ba)
    + Extract the downloaded zip file.
    + Open the extracted folder in Visual Studio Code (VSC).
7.	Configure Firebase in the App
    + Navigate to public/js/firebase-config.js in VSC.
    + Replace the existing firebaseConfig with your project’s configuration.
    ![Configuration](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/e10b14b7-f529-4199-8e99-b79b3aa50697)
8.	Install Firebase SDK
    + Open a terminal in VSC.
    + Run the command: `$ npm install firebase`
9.	Update Firebase Project Name
    + Open the .firebaserc file.
    + Change the project name to your Firebase project’s name.
    ![Login1](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/02fc6670-32e6-42fe-8dfd-487c8715ceeb)
10.	Deploy the App to Firebase Hosting
    + In the terminal, log in to Firebase with: `$ firebase login`
    ![Login2](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/8744b400-9373-4ced-b9ba-e06bae50eea5)
    ![Login3](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/f2c96a08-4050-47e0-8faa-b5af1664dffc)
    ![Login4](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/7b17b0f6-f283-4b92-a45f-21392fc1aa24)
    + Deploy your app with: `$ firebase deploy`
    ![Deploy](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/76f9aead-c7d2-4d52-8d8b-30264f54f311)
11.	Serve the App Locally (Optional) 
    + Ensure you have the Firebase CLI installed. If not, run `$ npm install -g firebase-tools` to install it globally.
    + In your terminal, navigate to the root directory of your project.
    + Run the command: `$ firebase serve`
    ![ServingLocally](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/5807b6bf-dab8-4472-811f-61f38a29d55b)
    + This will start a local server. By default, the app will be served at 
    ```sh
    http://localhost:5000
    ```
    + Any changes made to the code will reflect automatically if you refresh the page, providing a smooth development workflow.
12.	Verify Deployment
    + Go to the Hosting tab in the Firebase Console.
    + You should see your latest deployments listed.
    ![HostingDashboard](https://github.com/if23b011/GuessTheFlagMultiplayer/assets/145259777/a13566dc-1b2a-4701-8142-60aa3c5dc51a)

