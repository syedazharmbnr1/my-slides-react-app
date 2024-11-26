# Slides React App

This React application showcases various slides, including the Traffic Forecast Model Evolution and Future Improvements.

## Setup Instructions

1. Ensure you have Node.js and npm installed on your system.
2. Navigate to the project directory in your terminal.
3. Run the following commands:

```bash
# Install dependencies
npm install

# Start the development server
export NODE_OPTIONS=--openssl-legacy-provider
npm start
```

## Steps to Fix the Deployment Issue

1. Set NODE_OPTIONS for OpenSSL Legacy Provider

Vercel requires an environment variable to resolve the OpenSSL error.
- In your Vercel project:
  1. Go to Settings > Environment Variables.
  2. Add a new environment variable:
     - Key: NODE_OPTIONS
     - Value: --openssl-legacy-provider
  3. Save the environment variable and redeploy the project.