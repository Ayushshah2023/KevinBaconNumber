# KevinBaconNumber

In this project, we explore the concept of the "Kevin Bacon number" which measures the degree of separation between Hollywood actors based on their collaborations in movies. Kevin Bacon himself is assigned a Kevin-Bacon number of 0. Any actor who has appeared in a movie with Kevin Bacon has a Kevin-Bacon number of 1. Actors who haven't appeared with Bacon but have worked with someone who has, have a Kevin-Bacon number of 2, and so on.

## Introduction

The goal of this project is to compute the Kevin-Bacon number for various actors and analyze the average distance of all actors to Kevin Bacon. By doing so, we test the theory of six degrees of separation in Hollywood, which suggests that most actors are connected to Kevin Bacon within six steps.

### Data

We'll be using various lists of movies and actors, including:
- BaconCast06.txt: movies released in 2006
- BaconCast00_06.txt: movies released since 2000
- BaconCastFull.txt: all movies
- ActionCast.txt: action movies
- PopularCast.txt: popular movies

Each line in the data files contains the name of a movie followed by the cast, with names separated by the '/' character.

## Project Structure

The project consists of the following tasks:
1. Reading and loading the data into an appropriate data structure.
2. Representing actor-movie relationships as a graph.
3. Computing Kevin-Bacon numbers using breadth-first search (BFS).
4. Finding the shortest alternating sequence of actor-movie pairs that lead to Kevin Bacon.

## Implementation Details

- **File:** bacon_number.py
- **Class:** BaconNumber
  - Methods:
    1. `__init__(self, data_file: str)` - Initializes the class with the provided data file.
    2. `load_data(self)` - Reads and loads the data into memory.
    3. `compute_bacon_number(self, actor_name: str) -> int` - Computes the Kevin-Bacon number for the given actor.
    4. `shortest_path_to_bacon(self, actor_name: str) -> List[str]` - Finds the shortest path to Kevin Bacon for the given actor.

## Conclusion

This project aims to analyze the interconnectedness of Hollywood actors through their movie collaborations. By computing Kevin-Bacon numbers and shortest paths, we contribute to the understanding of the small world phenomenon in the entertainment industry.

Have fun exploring the fascinating world of Hollywood connections!

