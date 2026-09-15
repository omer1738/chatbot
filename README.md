OmarGPT

A full-stack AI chatbot web app powered by Claude. Built from scratch as a way to learn full-stack development — covering frontend design, backend API handling, environment security, and deployment.

**Live demo:** 

## Features

- Real-time chat interface with a custom-designed UI
- Persistent conversation history (saved in the browser, survives refreshes)
- "New chat" option to reset the conversation
- Secure backend that keeps the API key off the client entirely
- Deployed as a single service (frontend + backend together)

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript (vanilla, no framework)
- **Backend:** Node.js, Express
- **AI:** Anthropic Claude API
- **Hosting:** Render

## How It Works

The frontend sends chat messages to a `/api/chat` endpoint on the backend. The backend attaches the API key (kept safely in an environment variable, never exposed to the browser) and forwards the request to Claude, then returns the response back to the frontend to display.

## What I Learned

This was my first full-stack project. Along the way I learned how frontend and backend communicate over HTTP, why API keys should never live in client-side code, how to manage environment variables, and how to deploy a Node.js app to a live server.
