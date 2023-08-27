# Degrees of Separation Program

This program, `degrees.py`, is designed to determine the number of degrees of separation between two individuals in a given dataset. It was developed as part of CS50's AI Week 0 project, which is a part of Harvard's computing course offered on edX.

The concept of "degrees of separation" is based on the idea that people are connected to each other through a network of relationships. In this context, the program calculates the shortest path of connections between two individuals, which indicates the number of steps it takes to reach from one person to another.

## Usage

To run the program, use the following command in your terminal:

```bash
python degrees.py dataset
```

Here, replace `dataset` with the name of the dataset file you want to use for calculations. The program will prompt you to enter the names of two individuals, and it will then determine the degrees of separation between them using the provided dataset.

## Dependencies

This program requires Python to be installed on your system. It does not have any external dependencies beyond the standard Python libraries.

## Dataset Format

The dataset should be in a specific format to be compatible with the program. Each line of the dataset should contain information about a relationship between two individuals. The format of each line should be as follows:

```
Name1, Name2, Year
```

- `Name1` and `Name2` are the names of the individuals connected in the relationship.
- `Year` is the year in which the relationship was established.

Ensure that the dataset file is located in the same directory as the `degrees.py` script when you run the program.

## How It Works

The program uses a graph-based approach to calculate the shortest path between two individuals. It constructs a graph using the relationships provided in the dataset and then employs a graph traversal algorithm, such as breadth-first search (BFS), to find the shortest path between the source and target individuals.

## Example

Suppose you have a dataset file named `small.csv`, and you want to determine the degrees of separation between "Alice" and "Bob." You can run the program as follows:

```bash
python degrees.py small
```

The program will prompt you to enter the names of the two individuals and then output the degrees of separation between them based on the provided dataset.

## Acknowledgments

This program was developed as a project for CS50's AI Week 0, a part of Harvard's CS50 Introduction to Artificial Intelligence with Python course on edX.

For any questions or issues related to the program, feel free to reach out
