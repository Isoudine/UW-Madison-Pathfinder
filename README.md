Path Finder Application
This is a Java application designed to calculate the shortest path between buildings using Dijkstra's algorithm. The application allows users to load data files representing graphs, calculate paths, and display statistics about the dataset.

Features
Load Graph Data: Load building and path data from a file.
Show Dataset Statistics: Display information about the number of buildings, paths, and total time.
Calculate Shortest Path: Compute the shortest path between two specified buildings.
Interactive Command-Line Interface: Simple text-based user interface for interacting with the application.
Getting Started
Prerequisites
Java 8 or later
JUnit 5 for testing
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/path-finder.git
cd path-finder
Compile the Java files:

bash
Copy code
javac -d bin src/*.java
Run the application:

bash
Copy code
java -cp bin Frontend
Usage
When you start the application, you will see the following menu options:

vbnet
Copy code
Welcome to Path Finder!
Please enter what command you would like to do:
(1) Load the file 
(2) Show data statistics
(3) Calculate shortest path
(4) Exit App
Commands
Load File (1): Enter the name of the file containing the graph data. The file should be in a specific format with nodes and edges.

Show Data Statistics (2): Display statistics about the loaded dataset, including the total number of buildings and paths.

Calculate Shortest Path (3): Enter the starting and destination buildings to calculate the shortest path between them.

Exit App (4): Exit the application.

Example
Load a file named campus.dot:

mathematica
Copy code
Enter file name: 
campus.dot
Show data statistics:

java
Copy code
Total buildings = 10
Total edges = 15
Calculate the shortest path from "Memorial Union" to "Education Building":

sql
Copy code
Enter start building: 
Memorial Union
Enter end building: 
Education Building

The Shortest Path is:
Go from Memorial Union to Education Building in 118.00 seconds
The total time to go from Memorial Union to Education Building is 118.00 seconds
Testing
The application includes JUnit tests to verify the functionality of the graph and frontend components. Run the tests using:

bash
Copy code
java -cp bin:lib/junit-platform-console-standalone-1.8.1.jar org.junit.platform.console.ConsoleLauncher --scan-class-path
Project Structure
Frontend.java: Handles user interaction and input.
Backend.java: Manages data loading, path calculation, and dataset statistics.
DijkstraGraph.java: Implements Dijkstra's algorithm for shortest path calculation.
Tests: Contains JUnit test classes for frontend and backend validation.
Contributing
Fork the repository.
Create a new branch for your feature or bug fix.
Commit your changes.
Push your branch and submit a pull request.
