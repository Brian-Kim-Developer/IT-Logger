# IT Logger

## Introduction

## Technologies
###
<br/>

## Commands | []: optional

### 1. Create React app
```npx create-react-app .```

### 2. Install required dependencies
```npm install -D json-server concurrently```

### 3. Change package.json file
```
{
  "name": "it_logger",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "react": "^16.11.0",
    "react-dom": "^16.11.0",
    "react-scripts": "3.2.0"
  },
  "scripts": {
    "start": "react-scripts start",
    "json-server": "json-server --watch db.json --port 5000", <-- This is added.
    "dev": "concurrently \"npm start\" \"npm run json-server\"", <-- This is added.
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "eslintConfig": {
    "extends": "react-app"
  },
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  },
  "devDependencies": {
    "concurrently": "^5.0.0",
    "json-server": "^0.15.1"
  },
  "proxy": "http://localhost:5000" <-- This is added.
}
```

### 4. Install CSS dependency
```npm install materialize-css```

### 5. Run dev script
```npm run dev```

### 6. Remove files from root directory
```App.test.js```<br/>
```index.css```<br/>
```logo.svg```<br/>
```serviceWorker.js```

### 7. Install moment dependencies
```npm install moment react-moment```

### 8. Install Redux dependencies
```npm install redux react-redux redux-thunk redux-devtools-extension```<br/>
```redux``` is a state management library, which has nothing to do with react itself.<br/>
```react-redux``` allows us to connect the two together and they work really well together.<br/>
```redux-thunk``` is a piece of middleware and allows us to make asynchronous functions inside of our actions so that we can for instance wait for a response to come back and then dispatch to our reducer.<br/>
```redux-devtools-extension``` is for Chrome.

