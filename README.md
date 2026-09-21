# TRACE

> **Follow the evidence. Escape the pursuit.**

TRACE is a browser-based 2D investigation game inspired by forensic investigation, pursuit scenarios and linguistic evidence.

The player navigates through a maze, collects evidence and tries to avoid an autonomous police unit. The project combines game development, pathfinding, AI concepts and full-stack web development.

The project also connects my background in linguistics with software development and my interest in forensic investigation.

---

## 🚧 Project Status

**Work in progress**

TRACE is currently in early development.

### Current focus

- [ ] Set up game canvas
- [ ] Create maze
- [ ] Implement player movement
- [ ] Implement collision detection
- [ ] Add evidence items
- [ ] Add police entity
- [ ] Implement A\* pathfinding
- [ ] Add game states
- [ ] Add score system
- [ ] Add multiple levels
- [ ] Add backend
- [ ] Add database
- [ ] Add investigation/case system
- [ ] Add linguistic analysis features

---

## 🎮 Concept

TRACE is a 2D maze-based pursuit game with an investigation theme.

The player enters an investigation scene, collects evidence and attempts to escape an autonomous police unit.

The initial game loop is:

```text
Enter case
    ↓
Explore maze
    ↓
Collect evidence
    ↓
Avoid pursuit
    ↓
Collect enough evidence
    ↓
Solve case
```

The police unit uses autonomous movement and pathfinding to pursue the player.

---

## 🧩 Planned Features

### Core Game

- Grid-based maze
- Player movement
- Collision detection
- Collectible evidence
- Score system
- Timer
- Win / lose conditions
- Multiple levels

### Police AI

- Autonomous police movement
- A\* pathfinding
- Dynamic path recalculation
- Player pursuit
- Different AI behaviours

### Investigation

- Cases
- Evidence items
- Evidence types
- Case progress
- Investigation dashboard
- Case history

### Full-Stack Features

- User accounts
- Persistent game sessions
- Player statistics
- High scores
- Case data
- Evidence data

### Future Linguistics / Speech Features

The long-term goal is to experiment with linguistic and speech-related data.

Possible future features include:

- Text evidence
- Interview transcripts
- Linguistic feature extraction
- Keyword analysis
- Named entity recognition
- Stylometric features
- Audio evidence
- Speech-to-text
- Speech analysis

These features are planned extensions and are not part of the initial game version.

---

## 🛠️ Tech Stack

### Frontend

- React
- TypeScript
- HTML Canvas
- Vite

### Game

- TypeScript
- Grid-based game world
- Collision detection
- A\* pathfinding

### Backend

Planned:

- Node.js
- Express
- REST API
- WebSockets / Socket.IO

### Database

Planned:

- PostgreSQL

### Testing

Planned:

- Vitest
- React Testing Library

---

## 🏗️ Planned Architecture

```text
                         TRACE
                           │
             ┌─────────────┴─────────────┐
             │                           │
             ▼                           ▼
        React Frontend              Backend API
             │                           │
      ┌──────┴──────┐              ┌─────┴─────┐
      │             │              │           │
      ▼             ▼              ▼           ▼
   Game UI       Canvas         Game Data   Authentication
                    │
                    ▼
              Game Engine
                    │
        ┌───────────┼───────────┐
        │           │           │
        ▼           ▼           ▼
     Player      Police      Evidence
                    │
                    ▼
               A* Pathfinding
                           │
                           ▼
                      PostgreSQL
```

React is responsible for the user interface, while the game engine manages the real-time game state, movement, collisions and AI behaviour.

---

## 🧠 Game AI

The police unit is planned to use **A\* pathfinding** to find a route through the maze towards the player.

The maze is represented as a grid:

```text
################
#..............#
#.######.......#
#..............#
#......####....#
#..............#
################
```

Where:

```text
# = wall
. = walkable tile
```

The pathfinding algorithm operates on the grid rather than directly on screen coordinates.

---

## 🔍 Forensic / Linguistic Concept

TRACE is inspired by the idea of following and analysing different types of evidence.

For example:

```text
CASE 404

Evidence
────────────────────

[TEXT]  Witness statement
[AUDIO] Anonymous phone call
[IMAGE] CCTV image
[TEXT]  Written note
```

A future version may allow text and audio evidence to be analysed using NLP and speech-processing techniques.

The forensic elements are intended as a thematic and educational context for the software project. The application is not intended to provide real-world forensic conclusions.

---

## 📁 Project Structure

```text
src/
├── components/
│   ├── GameCanvas.tsx
│   ├── Score.tsx
│   ├── Timer.tsx
│   └── GameOver.tsx
│
├── game/
│   ├── Game.ts
│   ├── GameState.ts
│   ├── Renderer.ts
│   ├── input.ts
│   │
│   ├── entities/
│   │   ├── Player.ts
│   │   ├── Police.ts
│   │   └── Evidence.ts
│   │
│   ├── maze/
│   │   ├── Maze.ts
│   │   └── levels.ts
│   │
│   └── pathfinding/
│       └── astar.ts
│
├── App.tsx
├── main.tsx
└── styles.css
```

The structure may change as the project evolves.

---

## 🚀 Getting Started

### Prerequisites

Make sure you have installed:

- Node.js
- npm
- Git

### Installation

Clone the repository:

```bash
git clone <YOUR_REPOSITORY_URL>
```

Navigate into the project:

```bash
cd trace
```

Install dependencies:

```bash
npm install
```

### Start the development server

```bash
npm run dev
```

Vite will start the local development server.

Open the URL shown in the terminal, usually:

```text
http://localhost:5173
```

---

## 🧪 Testing

Testing will be added as the project develops.

Planned test areas include:

- Maze validation
- Collision detection
- Player movement
- Evidence collection
- A\* pathfinding
- Game state transitions
- API endpoints

---

## 📈 Development Roadmap

### Phase 1 — Game Prototype

- [ ] Canvas setup
- [ ] Maze rendering
- [ ] Player
- [ ] Keyboard controls
- [ ] Collision detection

### Phase 2 — Game Mechanics

- [ ] Evidence collection
- [ ] Score
- [ ] Timer
- [ ] Win / lose conditions

### Phase 3 — Police AI

- [ ] Police entity
- [ ] Basic movement
- [ ] A\* implementation
- [ ] Dynamic pursuit
- [ ] Multiple AI behaviours

### Phase 4 — Full-Stack Application

- [ ] Backend API
- [ ] PostgreSQL database
- [ ] User accounts
- [ ] Game sessions
- [ ] Persistent scores

### Phase 5 — Investigation System

- [ ] Case management
- [ ] Evidence management
- [ ] Investigation dashboard
- [ ] Case history

### Phase 6 — Linguistics / Speech

- [ ] Text evidence
- [ ] Transcript data
- [ ] NLP analysis
- [ ] Linguistic features
- [ ] Audio evidence
- [ ] Speech-to-text
- [ ] Speech analysis

---

## 🎯 Learning Goals

This project is being developed as a practical learning project to explore:

- TypeScript
- React
- Canvas-based game development
- Game loops
- State management
- Algorithms and data structures
- Graphs and pathfinding
- A\* search
- AI behaviour
- REST APIs
- WebSockets
- PostgreSQL
- Authentication
- Testing
- NLP
- Speech technology

---

## 📚 Project Background

TRACE combines three areas of interest:

```text
Linguistics
     +
Software Development
     +
Forensic Investigation
     ↓
    TRACE
```

The long-term goal is to use software development skills to explore applications related to computational linguistics, NLP, speech technology and forensic linguistics.

---

## 📸 Screenshots

Screenshots and gameplay recordings will be added as the project develops.

---

## 📄 License

This project is currently a personal learning project.

License information will be added later.
