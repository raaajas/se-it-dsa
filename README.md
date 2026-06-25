# SE IT - Data Structures & Algorithms (DSA) Programs

A structured collection of C/C++ programs implementing core Data Structures and Algorithms. These programs are aligned with the Savitribai Phule Pune University (SPPU) Second Year Information Technology (SE IT) curriculum.

![C++](https://img.shields.io/badge/C++-00599C?logo=c%2B%2B&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?logo=c&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)

---

## 📂 Repository Contents & Directory Map

The programs in this repository are divided into core data structure categories, Unix systems programming, and competitive programming helpers.

### 1. Core Data Structures & Sorting

| Program / File | Data Structure / Algorithm | Description | Complexity (Worst/Average) |
| :--- | :--- | :--- | :--- |
| **[assignment1.cpp](assignment1.cpp)** | Array of Structures / Bubble, Insertion, Quick Sort | Manages a student database. Sorts records by roll number (Bubble), alphabetically (Insertion), and outputs the top 10 toppers (Quick Sort). Implements Linear & Binary Search. | $O(N^2)$ (Bubble/Insertion), $O(N \log N)$ (Quick Sort) |
| **[assignment2.cpp](assignment2.cpp)** | Stack ADT (Linked List) | Converts infix expressions to postfix and evaluates postfix expressions using a stack. | Time: $O(N)$ \| Space: $O(N)$ |
| **[circularQ.cpp](circularQ.cpp)** | Circular Queue (Array) | Implements queue insertion, deletion, and display operations in a circular fashion to optimize memory reuse. | Time: $O(1)$ (Enqueue/Dequeue) |
| **[binary_search_tree.cpp](binary_search_tree.cpp)** | Binary Search Tree (BST) | Performs insertion, deletion, node search, depth calculation, leaf counting, displaying values, and creating a mirror tree image. | Time: $O(H)$ where $H$ is Tree Height |
| **[threaded_binary_tree.cpp](threaded_binary_tree.cpp)** | Threaded Binary Tree (TBT) | Implements an inordered threaded binary tree with insertion and inorder traversal without recursion or stacks. | Traversal: $O(N)$ \| Space: $O(1)$ |
| **[expression_tree.cpp](expression_tree.cpp)** | Expression Tree | Builds an expression tree from prefix/postfix expressions. Performs recursive and non-recursive traversals (Inorder, Preorder, Postorder). | Time: $O(N)$ |
| **[max_min_heap.cpp](max_min_heap.cpp)** | Heap / Heap Sort | Uses Max Heap and Min Heap representation to sort and find the maximum/minimum student marks. | Time: $O(N \log N)$ (Heap Sort) |

### 2. Graph Algorithms & Disjoint Sets

| Program / File | Algorithm | Description | Complexity |
| :--- | :--- | :--- | :--- |
| **[kruskal’s_prim's.cpp](kruskal’s_prim's.cpp)** | Prim's & Kruskal's Algorithms | Computes the Minimum Spanning Tree (MST) of a connected graph representing telephone lines or road networks. | $O(V^2)$ (Prim's), $O(E \log E)$ (Kruskal's) |
| **[Kruskal_Minimum_Spanning_Using_Disjoint_Set.cpp](Kruskal_Minimum_Spanning_Using_Disjoint_Set.cpp)** | Kruskal's + DSU | Optimized Kruskal's MST algorithm utilizing Disjoint Set Union (DSU) with path compression. | $O(E \alpha(V))$ where $\alpha$ is Inverse Ackermann |
| **[dijkstra's.cpp](dijkstra's.cpp)** | Dijkstra's Algorithm | Computes the single-source shortest path on a weighted graph. | $O(V^2)$ (Adjacency Matrix) |
| **[dsu.cpp](dsu.cpp)** | Disjoint Set Union (DSU) | Helper module containing Disjoint Set data structures (`find` and `union` operations). | $O(\alpha(V))$ per operation |

### 3. File Handling & Sequential Access

| Program / File | Concept | Description |
| :--- | :--- | :--- |
| **[file_handeling.cpp](file_handeling.cpp)** | Sequential Files | Implements file storage for student records. Features record insertion, sequential display, searching, and deletion. |

### 4. Unix Systems & Inter-Process Communication (IPC)

| Program / File | Concept | Description |
| :--- | :--- | :--- |
| **[pipe_concat_strings.c](pipe_concat_strings.c)** | Unix Pipes (IPC) | Communicates between parent and child processes to concatenate two strings using unidirectional pipes. |
| **[pipe_reverse_string.c](pipe_reverse_string.c)** | Unix Pipes (IPC) | Demonstrates inter-process communication by passing a string from a parent to a child process, reversing it, and returning it. |
| **[exec.c](exec.c)** | System Calls | Demonstrates the usage of the Unix `exec()` system call family to load and run another program binary. |

### 5. Competitive Programming & Helper Scripts
- **[Kth_largest_element.cpp](Kth_largest_element.cpp)**: C++ program to find the K-th largest element in an array.
- **[interger_sort.c](interger_sort.c)**: Basic array sorting algorithm implemented in C.
- **[even_odd_sum.c](even_odd_sum.c)**: Simple program calculating sum of even and odd integers in an array.
- **[Three Boxes.dev](Three%20Boxes.dev)**: Dev-C++ project metadata file.
- **Python Scripts (`*.py`)**: Miscellaneous scripts (like `Alpha.py`, `Tshirtmazayenar.py`, `Faraknahipadat.py`) representing small challenges and coding puzzles.

---

## 🛠️ How to Compile and Run

Make sure you have `g++` (GCC compiler) installed on your system.

### C++ Compilation (Data Structures)
For compiling C++ programs:
```bash
# Compile
g++ binary_search_tree.cpp -o bst_demo

# Run
./bst_demo
```

### C Compilation (Unix / System Programs)
For compiling Unix systems and pipe scripts:
```bash
# Compile
gcc pipe_reverse_string.c -o pipe_demo

# Run
./pipe_demo
```
*Note: Unix pipe and system call files require a POSIX-compliant environment (Linux, macOS, or WSL on Windows) to execute successfully.*
