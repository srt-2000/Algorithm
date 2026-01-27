# Algorithms Collection

> Interactive collection of algorithms from "Grokking Algorithms" book with CLI interface

## 📋 Description

This project is a CLI application that demonstrates various algorithms described in the "Grokking Algorithms" book. 
Each algorithm is implemented as a separate command with an interactive interface.

##
This project helps us understand how various algorithms work using Python code and visualize their output.
You can use it as 'study code'. 

1. Look into code.
2. Think about - How does it work.
3. Try to make result with CLI app.

##
No running time benchmarks were created to compare different methods, 
as the main goal of the project is to translate the examples described in the book into Python code.

## 📁 Project Structure

```
Algorithm/
├── data/                    # Test data in JSON format
│   ├── 5_2_data.json
│   ├── 6_1_data.json
│   └── ...
├── src/                     # Algorithm implementations
│   ├── binary_search.py    # Binary search
│   ├── dijkstra.py         # Dijkstra's algorithm
│   ├── dynamic.py          # Dynamic programming
│   └── ...
├── main.py                 # CLI interface
├── pyproject.toml         # Poetry configuration
└── requirements.txt       # Dependencies
```

## 🛠 Installation

### Requirements
- Python 3.12+
- Poetry (recommended) or pip

### Installation via Poetry (recommended)

```bash
# Clone repository
git clone <repository-url>
cd Algorithm

# Install dependencies
poetry install

# Activate virtual environment
poetry shell
```

### Installation via pip

```bash
# Clone repository
git clone <repository-url>
cd Algorithm

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
venv\Scripts\activate  # Windows

# Install dependencies
pip install -r requirements.txt
```

## 🎯 Usage

### Basic Commands

```bash
# Show all available commands
python main.py --help

# Run specific algorithm
python main.py <command_name>
```

### 📚 Available Algorithms

#### 🔍 Search and Sorting
- **`bs`** - Binary Search
  ```bash
  python main.py bs --mx 100 --find 42
  ```

- **`qsr`** - Quick Sort
  ```bash
  python main.py qsr
  ```

#### 🌳 Trees and Graphs
- **`bt`** - Binary Tree Traversal
  ```bash
  python main.py bt --ptype pre  # pre|post|in
  ```

- **`dk`** - Dijkstra's Algorithm
  ```bash
  python main.py dk
  ```

- **`ws`** - Breadth-First Search (BFS)
  ```bash
  python main.py ws --name Alex
  ```

#### 🧮 Dynamic Programming
- **`dc`** - Knapsack Problem
  ```bash
  python main.py dc
  ```

#### 🔐 Cryptography
- **`dh`** - Diffie-Hellman Protocol
  ```bash
  python main.py dh --p 23 --g 5
  ```

- **`bf`** - Bloom Filter
  ```bash
  python main.py bf
  ```

#### 🎯 Machine Learning
- **`nn`** - k-Nearest Neighbors Algorithm
  ```bash
  python main.py nn
  ```

#### 📊 Data Processing
- **`fr`** - Fourier Transform
  ```bash
  python main.py fr
  ```

- **`ih`** - Inverted Index
  ```bash
  python main.py ih --word "algorithm"
  ```

#### 🗂 Hash Tables
- **`ht1`** - Voting System
  ```bash
  python main.py ht1 --qnt 5
  ```

- **`ht2`** - URL Caching
  ```bash
  python main.py ht2
  ```

#### 🔄 Recursion
- **`cr`** - Countdown
  ```bash
  python main.py cr --rng 10
  ```

- **`fc`** - Factorial Calculation
  ```bash
  python main.py fc --fn 5
  ```

- **`sm`** - Array Sum
  ```bash
  python main.py sm
  ```

#### 🧮 Functional Programming
- **`mp`** - Map Function
  ```bash
  python main.py mp
  ```

- **`rc`** - Reduce Function
  ```bash
  python main.py rc
  ```

- **`mm`** - Matrix Multiplication
  ```bash
  python main.py mm
  ```

#### 🎯 Greedy Algorithms
- **`gr`** - Postman Problem
  ```bash
  python main.py gr
  ```

## 📊 Test Data

The project includes ready test data in the `data/` folder:
- Graphs for pathfinding algorithms
- Arrays for sorting and searching
- Statistical data for ML algorithms
- Cryptographic parameters

## 🧪 Usage Examples

### Binary Search
```bash
$ python main.py bs
Hello!
I'm the binary search algorithm
I'll find the index of item you want very fast

Enter the maximum number of sorted array: 100
Enter the digit we want to find: 42

We have a sorted list from 0 to 100
FIND!!!
42 is position of 42
```

### Dijkstra's Algorithm
```bash
$ python main.py dk
We have a graph with different paths to get our point:
{'start': {'a': 6, 'b': 2}, 'a': {'fin': 1}, 'b': {'a': 3, 'fin': 5}, 'fin': {}}

I've used the DSA Dijkstra's Algorithm and found our minimal trip
['start', 'b', 'a', 'fin']
```

## 👨‍💻 Author

**srt-2000** - [srt2000888@gmail.ru](mailto:srt2000888@gmail.ru)

## 🙏 Acknowledgments

- "Grokking Algorithms" book by Aditya Bhargava
---

⭐ If the project was helpful, give it a star!
