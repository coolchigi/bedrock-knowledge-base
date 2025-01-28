# Building a Knowledge Base with Amazon Bedrock

## Table of Contents

1. [Introduction](#introduction)
2. [Key Features](#key-features)
3. [Getting Started](#getting-started)
4. [Configuration](#configuration)
5. [How to Get Your Keys](#how-to-get-your-keys)
   - [Anthropic API Key](#anthropic-api-key)
   - [AWS Access Key and Secret Key](#aws-access-key-and-secret-key)
6. [Amazon Bedrock RAG Integration](#amazon-bedrock-rag-integration)
7. [Service Role](#service-role)
8. [Customized Deployment and Development](#customized-deployment-and-development)
9. [NPM Scripts](#npm-scripts)
10. [Appendix](#appendix)
11. [Disclaimer](#disclaimer)
12. [Source](#source)

## Introduction

RAG is a very common term in the AI world. It has become the buzz word at this point. When ChatGPT was introduced, LLMs were the buzz word. Now, it's RAG this, RAG that. What exactly is it? RAG stands for Retrieval Augmented Generation. It's a way to provide private context to LLMs. Common examples are those "help bots" you see on a company's webpage.

I've used quite a few apps that use RAG, and they're amazing! I can essentially chat with my PDFs, ask questions, and get answers. Google NotebookLM takes this to a whole new level! You can generate audio in a podcast style where two presenters discuss the PDFs or sources. I've always wanted to build one of these, but I never had the time to do so. This is for learning purposes, so I decided to leverage an existing app and maybe add a few tweaks here and there. My approach is, I am following the guide in the official repo and augumenting it with my knowledge or experience as I build. There's also a mini-challenge section that will help you understand the codebase better.

## Key Features

- AI-powered chat using Anthropic's Claude model & any model of your choice
- Amazon Bedrock integration for contextual knowledge retrieval
- Real-time thinking & debug information display
- Knowledge base source visualization
- User mood detection & appropriate agent redirection
- Highly customizable UI with shadcn/ui components
- Deployed on vercel!

## Mini-Challenge

### 1. UI Enhancement - Theme Management (Beginner)

**Task:** Add new themes to the UI
**Problem:** The dropdown menu becomes unwieldy with many themes
**Challenge:** Implement a scrollable or paginated theme selector
**Files to explore:**

- `components/TopNavBar.tsx`
- `styles/themes.js`

### 2. Source Attribution (Intermediate)

**Task:** Add source references to retrieved data
**Goal:** Show where the information comes from
**Suggestions:**

- Add line numbers
- Include file names
- Show context snippets
  **Files to explore:**
- `pages/api/chat.ts`
- `lib/bedrock.ts`

### 3. Advanced Features (Expert)

**Task:** Choose one:

- Implement chat history persistence
- Add support for multiple knowledge bases
- Create a custom theme builder

### Tips 💡

- Use the browser console to debug theme changes
- Review AWS Bedrock documentation for RAG implementation details

## Getting Started

1. Clone this repository.
2. Install dependencies: `npm install`
3. Set up your environment variables (see Configuration section).
4. Run the development server: `npm run dev`
5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Source

This project is based on code from [Anthropic Samples](https://github.com/anthropics/anthropic-quickstarts).
