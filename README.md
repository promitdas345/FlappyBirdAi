# Flappy-Bird-AI

AI learns to play Flappy Bird using NEAT (NeuroEvolution of Augmenting Topologies) algorithm.

## Features

- 1000 AI birds learning to play Flappy Bird through genetic evolution
- NEAT algorithm with speciation and innovation tracking
- Auto-save to localStorage with export/import to JSON files
- Full-screen responsive canvas
- Speed controls for faster training
- Multiple viewing modes and neural network visualization
- Comprehensive UI with real-time stats

## How to Run

1. **Navigate to the project folder:**
   ```bash
   cd Flappy-Bird-AI/flappyBird
   ```

2. **Start a local web server:**
   
   **Using Python:**
   ```bash
   python -m http.server 8000
   ```
   
   **Or using Node.js:**
   ```bash
   npx http-server -p 8000
   ```

3. **Open your browser and go to:**
   ```
   http://localhost:8000
   ```
   or
   ```
   http://127.0.0.1:8000
   ```

4. **Watch the AI learn!** The birds will get progressively better at navigating pipes over generations.

## Keyboard Controls

- **SPACE** - Toggle between showing all birds or just the best one
- **F** - Speed up training (increase FPS by 30)
- **S** - Slow down training (decrease FPS by 30)
- **N** - Hide graphics for super-fast training
- **B** - Replay the best AI bird
- **G** - Show best bird from each generation
- **P** - Play manually (you control the bird)
- **E** - Export best AI to JSON file
- **I** - Import AI from JSON file
- **L** - Manually save current best AI
- **D** - Delete saved AI data

## How It Works

The AI uses **NEAT** (NeuroEvolution of Augmenting Topologies), a genetic algorithm that evolves neural networks:

1. **Population**: 1000 birds start with random neural networks
2. **Inputs**: Each bird sees 4 values - vertical velocity, distance to pipe, height above bottom pipe, distance below top pipe
3. **Output**: Decision to flap or not (based on neural network)
4. **Fitness**: Birds that survive longer and score higher have better fitness
5. **Selection**: Best birds reproduce to create the next generation
6. **Mutation**: Networks evolve through mutation (new connections, nodes, weight changes)
7. **Speciation**: Similar networks are grouped to protect innovation

Over generations, the birds learn to navigate through pipes!

## Technologies Used

- **p5.js** - Graphics and game loop
- **JavaScript** - Core game logic and NEAT implementation
- **HTML5 Canvas** - Rendering
