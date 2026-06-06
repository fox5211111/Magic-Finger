<div align="center">
<h1>Magic Finger</h1>
<p>AI-Powered Gesture-Controlled Bubble Shooter</p>
</div>

## Overview

Magic Finger is an interactive bubble shooter game that combines webcam-based hand gesture tracking with AI-driven strategic analysis. Use hand pinch gestures to aim and shoot, while the integrated AI assistant analyzes the board state and recommends optimal moves in real time.

## Features

- **Gesture Control**: Hand tracking via MediaPipe — pinch and pull to aim, release to shoot
- **AI Strategy Engine**: Real-time board analysis with color and target recommendations
- **Scoring System**: Multiple bubble colors with varying point values and combo multipliers
- **Physics-Based Gameplay**: Infinite bounce mechanics with collision detection
- **Responsive HUD**: Score tracking, color picker, and debug panel

## Tech Stack

- **React 19** with TypeScript
- **Vite** for fast development and building
- **MediaPipe Hands** for real-time hand tracking
- **Tailwind CSS** for UI styling
- **Lucide React** for icons

## Run Locally

**Prerequisites:** Node.js

1. Install dependencies:
   ```bash
   npm install
   ```

2. Set the `GEMINI_API_KEY` in [.env.local](.env.local):
   ```
   GEMINI_API_KEY=your-api-key-here
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

## Controls

| Gesture | Action |
|---------|--------|
| Open hand near ball | Grab the projectile |
| Pinch + Pull back | Draw the slingshot |
| Release pinch | Fire the shot |

## Project Structure

```
├── components/
│   └── MagicFinger.tsx    # Main game component with rendering & physics
├── services/
│   └── geminiService.ts   # AI strategy analysis service
├── types.ts               # Shared TypeScript interfaces
├── App.tsx                # Root application component
├── index.tsx              # Entry point
├── index.html             # HTML entry with CDN dependencies
├── package.json           # Project configuration
└── metadata.json          # App metadata & permissions
```
