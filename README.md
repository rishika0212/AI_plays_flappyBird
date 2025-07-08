# AI_plays_flappyBird

🐦 Flappy Bird AI – Evolving to Win!
Welcome to Flappy Bird AI – a fun project where a neural network learns to play Flappy Bird by itself using NEAT (NeuroEvolution of Augmenting Topologies).

No manual playing. No rage quits. Just watch a population of birds learn how to flap their way through endless pipes, getting better with every generation.

🎮 How It Works
We use Pygame to recreate the classic Flappy Bird game.

NEAT-Python evolves a neural network to control the bird’s jumps.

Each bird is controlled by its own neural network brain.

Over time, bad jumpers die out, better jumpers pass on their genes.

The goal? Survive longer. Pass more pipes. Score higher.

imgs/: All the game sprites – the bird animation, pipes, base, and background.

config-feedforward.txt: NEAT configuration file (adjust generations, population size, mutation rates, etc.)

flappy_bird_ai.py: The main game + NEAT logic.

⚙️ Tech Stack
🐍 Python 3

🎮 Pygame (for graphics and game physics)

🧠 NEAT-Python (for evolving neural networks)

🧬 How Does the AI Decide?
Each bird’s neural network takes:

Its current y-position

The vertical distance to the next pipe’s top

The vertical distance to the next pipe’s bottom

…and predicts whether to jump or not jump.

If the output is greater than 0.5, the bird flaps.

🚀 How to Run It
1️⃣ Install dependencies:

bash
Copy
Edit
pip install pygame neat-python
2️⃣ Make sure you have all images in the imgs folder.

3️⃣ Run the game:

bash
Copy
Edit
python flappy_bird_ai.py
Watch the evolution happen right in front of you! 🧠✨

🏆 How Does It Learn?
Fitness Function: Birds earn points for staying alive and passing pipes.

Bad birds (who hit pipes or the ground) lose fitness.

Good birds (who fly longer and pass more pipes) gain fitness.

Over generations, NEAT evolves better neural networks.

📈 What You’ll See
At first, all the birds will fail miserably (it’s hilarious).
But be patient! Within a few generations, you’ll notice smarter flapping, smoother flying, and better scores.
