# Flappy-Bird-AI

AI learns to play Flappy Bird using NEAT (NeuroEvolution of Augmenting Topologies) - a genetic algorithm that evolves neural networks.

## Quick Start

1. Navigate to the project folder:
   ```bash
   cd Flappy-Bird-AI/flappyBird
   ```

2. Start a local server (prints the URL in the terminal):
   ```bash
   python -m http.server 8000 --bind 127.0.0.1
   ```

3. Open the printed link (http://127.0.0.1:8000/)

## Controls

| Key | Action |
|-----|--------|
| **SPACE** | Toggle show all/best bird |
| **F / S** | Speed up / slow down |
| **N** | Hide graphics (faster training) |
| **B** | Replay best AI |
| **E / I** | Export / Import AI |
| **P** | Play manually |

## How It Works

- **Population**: 1000 birds with random neural networks
- **Inputs**: Velocity, distance to pipes, height gaps
- **Output**: Flap or don't flap
- **Evolution**: Best performers reproduce, mutations create variety
- **Speciation**: Similar networks grouped to protect innovation

Birds improve each generation by learning from successful strategies!

## Features

- Auto-save to localStorage
- Export/import trained AI as JSON
- Full-screen responsive canvas
- Real-time stats and neural network visualization
- Speed controls for rapid training
