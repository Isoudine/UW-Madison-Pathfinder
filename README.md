# UW-Madison Path Finder Application

This is a Java application designed to calculate the shortest path between University buildings using Dijkstra's algorithm. The application allows users to load data files representing graphs, calculate paths, and display statistics about the dataset.

## Features

- **Load Graph Data:** Load building and path data from a file.
- **Show Dataset Statistics:** Display information about the number of buildings, paths, and total time.
- **Calculate Shortest Path:** Compute the shortest path between two specified buildings.
- **Interactive Command-Line Interface:** Simple text-based user interface for interacting with the application.

## Getting Started

### Prerequisites

- Java 8 or later
- JUnit 5 for testing

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-repo/path-finder.git
    cd path-finder
    ```

2. **Compile the Java files:**

    ```bash
    javac -d bin src/*.java
    ```

3. **Run the application:**

    ```bash
    java -cp bin Frontend
    ```

## Usage

When you start the application, you will see the following menu options:

```plaintext
Welcome to Path Finder!
Please enter what command you would like to do: 
(1) Load the file 
(2) Show data statistics
(3) Calculate shortest path
(4) Exit App

1

Enter file name: or press 4 
campus.dot

File was loaded successfully!

Welcome to Path Finder!
Please enter what command you would like to do: 
(1) Load the file 
(2) Show data statistics
(3) Calculate shortest path
(4) Exit App

3

Enter start building: 
Memorial Union
Enter end building: 
Union South

The Shortest Path is:
Go from Memorial Union to Radio Hall in 176.70 seconds
Go from Radio Hall to Education Building in 113.00 seconds
Go from Education Building to South Hall in 187.60 seconds
Go from South Hall to Law Building in 112.80 seconds
Go from Law Building to X01 in 174.70 seconds
Go from X01 to Luther Memorial Church in 65.50 seconds
Go from Luther Memorial Church to Noland Hall in 183.50 seconds
Go from Noland Hall to Meiklejohn House in 124.20 seconds
Go from Meiklejohn House to Computer Sciences and Statistics in 164.20 seconds
Go from Computer Sciences and Statistics to Union South in 176.00 seconds
The total time to go from Memorial Union to Union South is 1478.20 seconds
```
## Testing

The application includes JUnit tests to verify the functionality of the graph and frontend components. Run the tests using:

```bash
java -cp bin:lib/junit-platform-console-standalone-1.8.1.jar org.junit.platform.console.ConsoleLauncher --scan-class-path
