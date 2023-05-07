# PWA-Text-Editor

- This is a Progressive Web Application (PWA) text editor that uses IndexedDB to create an object store and includes both GET and PUT methods. The application works without an internet connection, automatically saves content inside the text editor when the DOM window is unfocused, and is bundled with webpack.

## Installation

Clone this repository
Run npm install to install the required dependencies
Run npm run build to build the application with webpack
Run npm start to start the server
Navigate to http://localhost:3000 in your web browser

## Usage

### Offline Usage

- The application works offline, so you can use it without an internet connection. The application will automatically save your content inside the text editor when the DOM window is unfocused, so you don't need to worry about losing your work.

### Online Usage

When online, the application will communicate with the server to retrieve and store data in the IndexedDB object store.

To create a new document, click the "New Document" button. To load an existing document, click the "Open Document" button and select the document you want to open.

To save your changes, click the "Save" button. To close the document, click the "Close" button

### Progressive Web Application

You can install this application as a Progressive Web Application (PWA) on your device. To do this:

Open the application in your web browser
Click the "Install" button in the address bar (or in the menu, depending on your browser)
Follow the instructions to install the application
The application should now be installed on your device and accessible from your home screen or app drawer


## Technical Details 

### IndexedDB
The application uses IndexedDB to create an object store for storing and retrieving data. The object store has both GET and PUT methods, which allows the application to retrieve and store data in the IndexedDB object store.

### Bundling with Webpack
The application is bundled with webpack, which is a module bundler for JavaScript. The application's code is written in modern JavaScript using async/await syntax, which is transpiled with Babel to ensure compatibility with older browsers.

#### Service Worker with Workbox
The application uses Workbox to create a service worker that caches static assets. This allows the application to load faster and work offline, even when there is no internet connection.

### WebpackPwaManifest
The application uses the WebpackPwaManifest plugin to generate a manifest.json file, which is used by the browser to install the application as a Progressive Web Application (PWA). The manifest.json file includes information about the application, such as the name, icons, and theme color.