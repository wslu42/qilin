# Qilin
![qilin](https://user-images.githubusercontent.com/29524895/135762834-b42ec035-03ec-4d74-9777-e0e5ac7cfd13.png)
#### Play Qilin from you browser [at itch.io here](https://wslu42.itch.io/qilin).
As I am improving this game to add the increasing level difficulties, tutorials and storyline, comments and/or feedbacks are very welcomed!

## Story of this game

## History of this game
- An earlier version of is game in pygame named [qShooter can be found here](https://github.com/wslu42/qShooter).
- This work is inspired by QPong made by qiskit advocate [Junye Huang](https://huangjunye.github.io/), a quantum variant of classical Pong. [Play QPong here](https://alfa871212.itch.io/qpong).
- Quantum simulation in this game is done with [micro-qiskit code for LUA](https://github.com/qiskit-community/MicroQiskit/blob/main/versions/Lua/README.md)
- Game dev/Art/SFX all in [PICO-8](https://www.lexaloffle.com/pico-8.php).
- A solo game dev done by [Wen-Sen Lu](https://github.com/wslu42) during the [2021 itch.io Online Quantum Game Jam event](https://itch.io/jam/online-quantum-game-jam).

## Quantum ideas involved in this game
In this work I implemented randomness, superposition and entanglement through QASM backend (micro-qiskit for LUA, specifically). The user control is just a three-qubit circuit composer with circuit depth = 3, and by using X, H, and CX gates we asked user to come up with states match to the falling enemies.

The idea that I am experimenting is how to represent in-game locations with quantum states. In Qilin this is realized in controlling where the laser beams are shooting. It requires proficient understanding of 3-qubit states and the player's fast response to put together a quantum circuit which maps to the enemy's location using circuit composer. The goal is simple - shoot down as many as enemies as you can!

## Relevance of this game to the theme QUANTUM DA VINCI


## More behind the scene
The measurement part of in this code is designed such that counts won't be too high that user can basically shoot down anything with H gates.
1. Has only 16 shots each time when user load the circuit with space bar.
2. For states with counts <4, set the count of that state to 0.

## A detail walkthrough for gameplay
![Picture1](https://user-images.githubusercontent.com/29524895/135765697-42ebe447-65fb-43d9-8267-45b225a4ad44.png)
![Picture2](https://user-images.githubusercontent.com/29524895/135765698-1f1fa90e-56d3-4c56-aa6c-5dfb8322e681.png)
![Picture3](https://user-images.githubusercontent.com/29524895/135765701-e5c83a38-f7e2-40ba-a3aa-7ad79cf2551b.png)
![Picture4](https://user-images.githubusercontent.com/29524895/135765711-fa0e0bc7-94d4-4995-a1e0-7007cf3df86b.png)
![Picture5](https://user-images.githubusercontent.com/29524895/135765798-7daf1252-e266-41b1-902d-a3a1bd914156.png)
