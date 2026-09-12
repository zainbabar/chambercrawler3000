# ChamberCrawler3000 (CC3K)

A terminal based roguelike written in modern C++, built by a team of three as the final project for CS246: Object Oriented Software Development at the University of Waterloo.

## Source Code Availability

This was a CS246 project at the University of Waterloo, and course staff don't let students post assignment solutions publicly since the project gets reused in later terms. This repo has no code or UML in it, just this writeup.

If you're a recruiter or hiring manager and want to go through the implementation in more depth, reach out and we're happy to talk through it.

## Overview

CC3K is a five floor dungeon crawler. You pick a race, explore chambers, fight enemies, drink potions, and collect gold, trying to make it to the stairs on the fifth floor. Floors can be randomly generated or loaded from a layout file, and the game redraws after every command rather than updating in real time, closer to how the earliest roguelikes worked.

The codebase is organized into a character system, a world model, items, generation, and a display layer, built one class per module.

## Features

* Turn based dungeon exploration across five floors
* Five playable races and twelve enemy types, each with its own passive ability
* Combat where damage depends on both fighters' specific types, not just attacker vs defender stats
* Potions with hidden effects until first use, some temporary and some permanent
* Gold and treasure, including hoards guarded by dragons
* A toggleable inventory system for picking up potions and using them later (extra credit)
* Randomized enemy, item, and gold placement, or a fixed layout loaded from file
* Restart and game over handling

## Extra Credit Features

* A toggleable inventory system, so potions can be picked up and used later instead of only on the spot
* Smart pointers used across every ownership relation in the codebase, with no raw `delete` anywhere

## Technologies

* C++20, built with modules split into interface and implementation files
* RAII, smart pointers, virtual dispatch, and operator overloading throughout

## Software Engineering Concepts

* Object oriented design: encapsulation, inheritance, polymorphism, abstraction
* Design patterns: **Template Method**, **Decorator**, **Observer**, **Strategy**, **Factory Method**
* Modular architecture, one class per module for cohesion
* Git for collaboration, working across branches with a shared Makefile

---
Coursework from the University of Waterloo, described here for portfolio purposes only. No assignment code or UML is reproduced.
