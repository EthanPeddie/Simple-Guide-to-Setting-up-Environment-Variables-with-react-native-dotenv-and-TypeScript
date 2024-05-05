
# Simple Guide to Setting up Environment Variables with react-native-dotenv and TypeScript

## Overview

'react-native-dotenv' helps manage environment variables in React Native projects. Follow these easy steps to set it up with TypeScript for type safety.


## Step 1: Install react-native-dotenv

Open Terminal or Command Prompt.

Go to your React Native project folder:

```bash
  cd your-project-folder
  npm i react-native-dotenv
```

## Step 2: Configure Babel Plugin

Find babel.config.js in your project's root folder.
Add this configuration inside the plugins array:

```bash
  module.exports = {
  presets: ['module:metro-react-native-babel-preset'],
  plugins: [
    [
      'module:react-native-dotenv',
      {
        envName: 'APP_ENV',
        moduleName: '@env',
        path: '.env',
      },
    ],
  ],
};

```

## Step 3: Define Environment Variables
Create a '.env' file in your project's root folder.

Add your environment variables in the format KEY=VALUE. For example:

```bash
 API_URL=https://example.com/api
 API_KEY=your-api-key
```

## Step 4: Access Environment Variables
Use the '@env' module to access environment variables in your TypeScript files:

```bash
 import { API_URL, API_KEY } from '@env';

console.log(API_URL); // Output: https://example.com/api
console.log(API_KEY); // Output: your-api-key

```

## Step 5: Add Type Declarations (Optional)
Create a types folder in src if not already present.

Inside types, create env.d.ts.

Add type declarations for your environment variables:

```bash
 declare module '@env' {
  export const API_URL: string;
  export const API_KEY: string;
}
```

## That's It!

You've successfully set up environment variables with 'react-native-dotenv' and TypeScript in your React Native project!
## Documentation

[Documentation](https://www.npmjs.com/package/react-native-dotenv)


## License

[MIT](https://github.com/EthanPeddie)
