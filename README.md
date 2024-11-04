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
I started experimenting with different ideas a couple of months ago. While studying for a course, I had a light bulb moment: "What if I implement my own chat-with-documents app?"

I've used quite a few of these apps, and they're amazing! I can generate questions based on a particular section or topic. It's pretty cool 🤯

I sat back at the drawing board and remembered reading an article about Amazon Bedrock some months back. I thought, "Hmm, let's explore." I wanted to build my own application, but the purpose of my exploration was to build fast. So I looked to see if it had been done before—and you bet it had! When using new tech or whatever the case may be, I like putting my own little spin on it.

## Key Features

- AI-powered chat using Anthropic's Claude model
- Amazon Bedrock integration for contextual knowledge retrieval
- Real-time thinking & debug information display
- Knowledge base source visualization
- User mood detection & appropriate agent redirection
- Highly customizable UI with shadcn/ui components
- Deployed on vercel!

## Getting Started

1. Clone this repository.
2. Install dependencies: `npm install`
3. Set up your environment variables (see Configuration section).
4. Run the development server: `npm run dev`
5. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Source

This project is based on code from [Anthropic Samples](https://github.com/anthropics/anthropic-quickstarts).
