# 3D Agent Monitor Dashboard

Visualize your OpenClaw agents in a real-time 3D world built with Three.js.

## What It Does

- Each OpenClaw agent becomes a **3D continent** with houses, trees, ponds, and nature
- Each session (group chat, private message, cron job, subagent) becomes a **cute minion** walking around
- Click any minion to see its **live conversation**, thinking process, and tool calls
- Send messages directly from the 3D view
- Real-time updates via Server-Sent Events (SSE)

## Tech Stack

- **Three.js** — 3D rendering with custom shaders (wind-swaying grass, water ripples, clouds)
- **Node.js + Express** — Backend server reading OpenClaw session files directly
- **SSE** — Real-time push updates (no polling)

## Key Features

| Feature | Description |
|---------|-------------|
| Physics | Gravity, drag-and-drop, collision detection (AABB) |
| Pathfinding | Smart movement to points of interest |
| Thinking Bubbles | Live "..." animation + mini speech bubble during processing |
| Notifications | Toast-style notification boxes for active sessions |
| Dual View Modes | Floating bubble or pinned bottom panel |
| Persistence | Server-side state persistence for minion positions |

## How to Use

```bash
git clone https://github.com/ccperdst-lab/openclaw-monitor.git
cd openclaw-monitor
npm install
npm start
# Open http://localhost:7777
```

## Links

- GitHub: [ccperdst-lab/openclaw-monitor](https://github.com/ccperdst-lab/openclaw-monitor)
