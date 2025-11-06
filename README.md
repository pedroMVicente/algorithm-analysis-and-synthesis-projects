# Algorithm Analysis and Synthesis Projects

A collection of three algorithmic problems solved as part of the Algorithm Analysis and Synthesis (ASA) course at Instituto Superior Técnico. Each project implements efficient solutions to complex computational problems with emphasis on time complexity, space optimization, and competitive programming techniques.

## 📚 Course Information

**Institution**: Instituto Superior Técnico  
**Course**: Análise e Síntese de Algoritmos (Algorithm Analysis and Synthesis)  
**Academic Year**: 2024/2025  
**Language**: C++ (primary), Python (Project 3)  
**Evaluation**: Mooshak automated testing system

---

## 🎯 Projects Overview

### Project 1: Binary Operator Parenthesization
**Deadline**: December 6, 2024

#### Problem Description
Archaeologist João Caracol discovered ancient tables defining binary operators and sequences of operations without parentheses. The challenge is to determine if it's possible to parenthesize a sequence of integers using a custom binary operator to achieve a desired result, and if so, output the leftmost valid parenthesization.

#### Key Concepts
- **Dynamic Programming**: Matrix chain multiplication variant
- **Custom Binary Operators**: Operator tables defining non-standard operations
- **Optimal Substructure**: Finding leftmost parenthesization
- **Complexity**: O(n³) time, O(n²) space

#### Input
- Operator table (n×n matrix)
- Sequence of m integers
- Target result value

#### Output
- `1` followed by leftmost parenthesization if possible
- `0` if no valid parenthesization exists

#### Example
```
Input:
2 4
1 2
2 1
1 2 2 1
1

Output:
1
(((1 2) 2) 1)
```

---

### Project 2: Metro Network Connectivity Index
**Deadline**: December 20, 2024

#### Problem Description
The municipality of Caracolândia commissioned a study to assess their metro network efficiency inspired by the 15-minute city concept. Calculate the metro connectivity (mc) index, which represents the maximum number of line changes needed to travel between any two stations in the network.

#### Key Concepts
- **Graph Theory**: Multi-graph representation of metro networks
- **Modified BFS**: Tracking line changes instead of distance
- **Connectivity Analysis**: Finding maximum minimum line changes
- **Special Cases**: Disconnected networks, single-line networks

#### Input
- n stations, m connections, l lines
- List of connections: station x, station y, line l

#### Output
- Metro connectivity index (maximum minimum line changes)
- `0` if no line changes needed
- `-1` if network is disconnected

#### Example
```
Input:
7 8 3
3 2 1
2 7 1
7 5 1
2 6 2
6 4 2
4 1 2
4 1 3
1 5 3

Output:
1
```

---

### Project 3: Santa's Toy Distribution Optimization
**Deadline**: January 9, 2025

#### Problem Description
Professor Natalino Caracol was hired by UbiquityInc (Santa's company) to optimize toy distribution worldwide. Factories produce specific toys with stock limits, countries have minimum delivery requirements and export limits, and children request toys. Maximize the number of satisfied children while respecting all constraints.

#### Key Concepts
- **Linear Programming**: Optimization with constraints
- **PuLP Library**: Python LP solver integration
- **Network Flow**: Resource allocation problem
- **Constraint Satisfaction**: Multiple constraint types

#### Input
- n factories, m countries, t children
- Factory specifications (location, stock)
- Country constraints (min deliveries, max exports)
- Children's toy requests

#### Output
- Maximum number of children that can be satisfied
- `-1` if constraints cannot be met

#### Implementation
- **Required**: Python with PuLP library
- **Solvers**: GLPK or LP_solve

---

## 🛠️ Technical Specifications

### Compilation & Execution

**C++ Projects (1 & 2)**
```bash
g++ -std=c++11 -O3 -Wall project.cpp -lm
./a.out < input.txt
```

**Python Project (3)**
```bash
python3 project.py < input.txt
```

### Requirements
- **Time Complexity**: Optimized for large inputs
- **Memory**: Limited by Mooshak system
- **I/O**: Standard input/output only
- **Implementation Time**: ~15 hours per project

### Dependencies (Project 3)
```bash
python -m pip install pulp
sudo apt-get install glpk-utils  # Ubuntu
```

---

## 📊 Project Structure

```
asa-projects-2024/
├── project1-parenthesization/
│   ├── project1.cpp
│   ├── report.pdf
│   └── test-cases/
├── project2-metro-connectivity/
│   ├── project2.cpp
│   ├── report.pdf
│   └── test-cases/
└── project3-toy-distribution/
    ├── project3.py
    ├── report.pdf
    └── test-cases/
```

---

## 📈 Evaluation Criteria

Each project is evaluated in two phases:

### Automated Testing (85%)
- Correctness verification via `diff` command
- Time and memory constraints
- Score range: 0-170 points
- Multiple test cases of increasing difficulty

### Report Evaluation (15%)
- Solution description and algorithm analysis
- Theoretical complexity analysis
- Experimental results and performance evaluation
- References and bibliography

### Report Requirements
- **Format**: PDF only
- **Length**: Maximum 2 pages
- **Font**: 12pt
- **Margins**: 3cm
- **Submission**: Fénix platform

---

## 🎓 Learning Outcomes

### Algorithmic Techniques
- Dynamic Programming
- Graph Algorithms (BFS, DFS)
- Linear Programming
- Greedy Algorithms
- Optimization Techniques

### Problem-Solving Skills
- Problem decomposition
- Complexity analysis (time and space)
- Edge case handling
- Efficient data structure selection

### Software Engineering
- Competitive programming standards
- Input/output optimization
- Memory-efficient implementations
- Code correctness and robustness

---

## 📝 License

These projects were developed as coursework for academic purposes at Instituto Superior Técnico.

---

## 👥 Author

Developed for the Algorithm Analysis and Synthesis course (2024/2025) at IST.

---

*Note: Test cases and detailed solutions are available after project deadlines. This repository showcases algorithmic problem-solving skills and optimization techniques learned throughout the course.*
