Neat-Python Game AI

This project uses NEAT (NeuroEvolution of Augmenting Topologies) to evolve neural networks that learn to play games automatically. Instead of writing rules for the player, the AI improves over generations through natural selection.

The repository includes AI agents that learn to play:

- Flappy Bird
- Chrome Dino–style runner

## How It Works

Each game agent is controlled by a neural network.

NEAT trains the AI by:

- Creating a population of random neural networks
- Letting each network control a game agent
- Assigning a fitness score based on performance
- Selecting the best networks to reproduce and mutate
- Repeating this process over many generations

No training data is required — learning happens through evolution.

## Setup and Installation

1. Clone the repository

```
git clone https://github.com/asd759/Neat-Python.git
cd Neat-Python
```

2. Create and activate a virtual environment

**macOS / Linux**
```
python3 -m venv venv
source venv/bin/activate
```

**Windows**
```
python -m venv venv
venv\Scripts\activate
```

3. Install dependencies

```
pip install -r requirements.txt
```

## Running the AI

**Flappy Bird AI**
```
python flappy_bird_ml/flappy.py
```

**Dino Game AI**
```
python Dino_game_2/dino.py
```

**Playable Dino Game**
```
python playable_dino_2.py
```

## NEAT Configuration

Each game uses a `config-feedforward.txt` file to control:

- Neural network inputs and outputs
- Mutation rates
- Population size
- Fitness thresholds

Changing these values affects how the AI learns.

## Requirements

- Python 3
- neat-python
- pygame

Exact versions are listed in `requirements.txt`.

## Notes

- Early generations may perform poorly — this is expected
- Closing the game window stops training
- This project is intended for learning and experimentation

## License

This project is licensed under the MIT License.
