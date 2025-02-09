Electron-App-Template
A template for quickly creating new Electron.js applications with React, TypeScript, and auto-updater support.

Getting Started
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/Dustin-Tripp/Electron_Template.git
2. Navigate into the Project Folder
bash
Copy
Edit
cd Electron_Template/Electron-App
3. Install Dependencies
bash
Copy
Edit
npm install
4. Run the App in Development Mode
bash
Copy
Edit
npm run dev
Configuration
Updating the App Name
The default application name is "electron-app". To rename it:

Open VS Code.
Use the global search (Ctrl + Shift + F / Cmd + Shift + F on Mac) for "electron-app".
Replace all instances with your new app name.
Setting Up Auto-Updates
Edit the electron-builder.yml file to enable auto-updates. Fill in your repository details:

yml
Copy
Edit
publish:
  provider: github
  owner: 'YOUR-GITHUB-USERNAME'
  private: true
  repo: 'YOUR-REPO-NAME'
  token: 'YOUR-GITHUB-TOKEN'
Building the Application
To compile and package the application, run:

bash
Copy
Edit
npm run build
For a Windows build, use:

bash
Copy
Edit
npm run build:win
The output will be located in the ./dist folder.

Auto-Update Requirements
For auto-updating to work, the following files must be included in your GitHub Releases:

✅ .exe
✅ .exe.blockmap
✅ latest.yml
