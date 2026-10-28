# Resume AI Chat

An AI-powered resume chatbot that allows users and recruiters to interact with a personal resume through natural language conversations. It uses Google's Gemini API to generate context-aware answers based on predefined resume information.

## Overview

Resume AI Chat transforms a traditional resume into an interactive experience. Instead of reading a static PDF, recruiters can ask questions about professional experience, technical skills, projects, education, and certifications.

## Features

- **AI-Powered Chat:** Ask questions about the resume in natural language.
- **Resume-Based Responses:** Generate answers using predefined resume information.
- **Suggested Questions:** Get started with predefined questions.
- **Interactive Chat UI:** Clean interface with message history and loading indicators.
- **Secure API Integration:** Keep Gemini API credentials on the server.
- **Resume Access:** Provide access to the resume PDF.
- **Deployment Ready:** Configured for deployment using Vercel.

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js serverless API
- **AI Model:** Google Gemini API
- **Hosting:** Vercel
- **Version Control:** Git and GitHub

## Project Structure

```text
resume-chat/
├── api/
│   └── chat.js
├── lib/
│   └── resume.js
├── public/
│   ├── index.html
│   └── resume.pdf
├── .env.example
├── .gitignore
├── package.json
└── vercel.json
```

## Getting Started

### Prerequisites

Before running the project, make sure you have:

- Node.js and npm installed
- A Google Gemini API key
- Vercel CLI installed

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd resume-chat
```

Replace `YOUR_GITHUB_REPOSITORY_URL` with your repository's actual URL.

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the project root and add:

```env
GEMINI_API_KEY=your_gemini_api_key
GEMINI_MODEL=your_supported_gemini_model_id
```

Replace the placeholder values with your actual credentials and a model ID supported by the Gemini API.

**Important:** Never upload your `.env` file or expose your API key in frontend code or a public GitHub repository.

### 4. Run Locally

Install the Vercel CLI if it is not already installed:

```bash
npm install -g vercel
```

Start the local development server:

```bash
vercel dev
```

Open the local URL displayed in your terminal to access the application.

## Deployment on Vercel

1. Push the project to a GitHub repository.
2. Log in to [Vercel](https://vercel.com/).
3. Import your GitHub repository.
4. Add the following environment variables under **Project Settings → Environment Variables**:
   - `GEMINI_API_KEY`
   - `GEMINI_MODEL`
5. Deploy the project.
6. Test the chat functionality after deployment.

If you update environment variables, redeploy the project for the changes to take effect.

## Custom Domain

The application can be connected to a custom domain.
