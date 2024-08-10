# Degrees
This project explores the concept behind the "Six Degrees of Kevin Bacon" game, which suggests that any actor in Hollywood can be connected to Kevin Bacon through six or fewer steps, where each step involves a film that two actors have both starred in. Here, we generalize the problem to find the shortest path between any two actors using a sequence of movies that connects them.

For example, the shortest path between Jennifer Lawrence and Tom Hanks is two steps:

Jennifer Lawrence starred in "X-Men: First Class" with Kevin Bacon.

Kevin Bacon starred in "Apollo 13" with Tom Hanks.

This problem is approached as a search problem:

States represent actors.
Actions are movies that connect one actor to another.
Initial State is the first actor.
Goal State is the second actor.
The project uses Breadth-First Search (BFS) to find the shortest path between two actors.

# Project Structure

Data: The project includes two datasets (large and small) consisting of CSV files for ease of testing and experimentation.

people.csv: Contains actor IDs, names, and birth years.

movies.csv: Contains movie IDs, titles, and release years.

stars.csv: Establishes relationships between actors and movies.

# Code:

degrees.py: Loads data from the CSV files, maps actor names and movies to IDs, and uses BFS to compute the shortest path between two actors based on their movie connections.

User Interaction: The user inputs two actor names, and the program outputs the shortest path between them, if one exists.

# How It Works

Data Loading: Information about actors and movies is loaded into memory from CSV files.

Search Execution: The shortest_path function implements BFS to find the shortest sequence of connections between two actors.

Result Output: The program prints the sequence of movies and actors that connect the two specified actors.

This project demonstrates an interesting application of search algorithms in a real-world context, showcasing how connections between people in the film industry can be analyzed using basic principles of computer science.
