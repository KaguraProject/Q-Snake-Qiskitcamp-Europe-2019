# Qiskit Camp Europe 2019 Hackathon: Q-Snake

## Introduction
In this project we have created a simple game based on the classical game of [Snake](https://en.wikipedia.org/wiki/Snake_(video_game_genre)). The project involves a combination of both python and qiskit (along with its reduced version, "aether") implemented on both software (via a simulator) and actual hardware (via a programmable console called the "Pew Pew"). The various modes implemented serve to introduce certain quantum computing and quantum mechanics concepts to anyone interested in the field using both a combination of Qiskit and Python. More importantly, the project also serves as a venue for enthusiasts interested in learning how to code with Qiskit. 

The following modes have been implemented:
+ Q-Python
+ Q-Python Plus
+ Q-Python Circuit

## Q-Python 
It is the simplest version of Q-Python and the only one that runs in the Pew Pew console (due to memory constraints). The game is similar to the classic game of Snake with the difference being the method by which the apples spawn. In the classic version, these apples are spawned randomly via a classical random generator. In the quantum version, this spawning is facilitated via a quantum random generator. This quantum random generator is implemented by performing measurement a qubit on a superposition. There is also a simple barrier mechanic that the snake can penetrate through quantum tunneling with some probability.

## Q-Python Plus
This mode is simliar to Q-Python but runs on a PewPew emulator due to the stated memory constraints. Again, the spawning of the apples are via quantum random generator. This mode, however, implementing more reastically through the actual equations and measurements made on qubits. This introduces concepts such as quantum tunneling and the bloch sphere. 

## Q-Python Circuit
This mode involves creating a 1 qubit quantum circuit with a specific goal in mind. The goal of the game is to reach a final state of ket 1 starting from an initial state of ket 0 (using the least amount of gates) given the limitation that one can only use H, Z, or measurement operations. As the snake eats apples, one is tasked to select one of the three available operations. Failure to select the correct gate at the right time will result in a game over. Additionally, the user must also avoid randomly generated noise.

## Licenses
The original snake game and the original pew simulator are taken from
https://github.com/pewpew-game
Creative Commons
Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) License
author: 2019 by Radomir Dopieralski

The compressed version of qiskit (aether) is taken from
https://github.com/quantumJim/aether
(Apache 2.0 licence)
author: quantumJim
