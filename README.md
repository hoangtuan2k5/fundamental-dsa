# Fundamental Data Structures and Algorithms (DSA)

[![.NET 8.0](https://img.shields.io/badge/.NET-8.0-blue.svg)](https://dotnet.microsoft.com/download)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DSA](https://img.shields.io/badge/Topic-Data%20Structures%20%26%20Algorithms-green.svg)](https://github.com/hoangtuan2k5/fundamental-dsa)
[![C#](https://img.shields.io/badge/Language-C%23-purple.svg)](https://docs.microsoft.com/en-us/dotnet/csharp/)
[![Author](https://img.shields.io/badge/Author-Hoàng%20Chiều%20Nguyễn%20Tuấn-orange.svg)](https://github.com/hoangtuan2k5)

A comprehensive C# implementation of fundamental data structures and algorithms, designed for educational purposes and practical understanding of computer science concepts.

## 📋 Table of Contents

- [Project Structure](#project-structure)
- [Data Structures](#data-structures)
  - [Arrays](#arrays)
  - [Linked Lists](#linked-lists)
  - [Stacks and Queues](#stacks-and-queues)
  - [Trees](#trees)
  - [Hash Tables](#hash-tables)
  - [Graphs](#graphs)
- [Algorithms](#algorithms)
  - [Search Algorithms](#search-algorithms)
  - [Sorting Algorithms](#sorting-algorithms)
  - [Dynamic Programming](#dynamic-programming)
- [Getting Started](#getting-started)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [License](#license)

## 🏗️ Project Structure

```
FundamentalDSA/
├── FundamentalDSA.Core/           # Core data structure implementations
├── FundamentalDSA.Examples/       # Usage examples and demonstrations
├── FundamentalDSA.Tests/          # Unit tests
├── FundamentalDSA.ConsoleApp/     # Console application for demonstrations
└── README.md
```

## 📊 Data Structures

### Arrays
- **Static Array**: Fixed-size array implementation with basic operations
- **Dynamic Array**: Resizable array with automatic capacity management

### Linked Lists
- **Single Linked List**: Linear data structure with nodes containing data and next pointer
- **Double Linked List**: Bidirectional linked list with previous and next pointers
- **Circular Single Linked List**: Single linked list where last node points to first
- **Circular Double Linked List**: Double linked list with circular connections

### Stacks and Queues
- **Stack (Array-based)**: LIFO data structure implemented using arrays
- **Stack (List-based)**: LIFO data structure implemented using linked lists
- **Queue (Array-based)**: FIFO data structure implemented using arrays
- **Queue (List-based)**: FIFO data structure implemented using linked lists

### Trees
- **Tree**: Basic tree structure with parent-child relationships
- **Binary Tree**: Tree where each node has at most two children
- **Binary Search Tree (BST)**: Binary tree with ordering property
- **AVL Tree**: Self-balancing binary search tree
- **Red-Black Tree**: Self-balancing binary search tree with color properties
- **Splay Tree**: Self-adjusting binary search tree
- **B-Tree**: Self-balancing search tree for sorted data
- **B+ Tree**: Variant of B-tree with all values stored in leaves

### Hash Tables
- **Hash Table**: Basic hash table implementation
- **Hash Functions**: Various hash function implementations
- **Separate Chaining**: Collision resolution using linked lists
- **Open Addressing**: Collision resolution using probing
  - **Linear Probing**: Sequential slot checking
  - **Quadratic Probing**: Quadratic function for slot checking
  - **Double Hashing**: Secondary hash function for probing

### Graphs
- **Graph**: Basic graph representation and operations
- **Adjacency Matrix**: 2D array representation
- **Adjacency List**: List-based representation

## 🔍 Algorithms

### Search Algorithms
- **Breadth-First Search (BFS)**: Level-by-level graph traversal
- **Depth-First Search (DFS)**: Deep exploration graph traversal
- **Uniform Cost Search**: Optimal path finding algorithm

### Sorting Algorithms
- **Bubble Sort**: Simple comparison-based sorting
- **Insertion Sort**: Efficient for small datasets
- **Selection Sort**: In-place comparison sorting
- **Quick Sort**: Divide-and-conquer efficient sorting
- **Merge Sort**: Stable divide-and-conquer sorting
- **Heap Sort**: Comparison-based sorting using heap
- **Radix Sort**: Non-comparison integer sorting

### Dynamic Programming
- **Dynamic Programming**: Optimization technique for overlapping subproblems

## 🚀 Getting Started

### Prerequisites
- [.NET 8.0 SDK](https://dotnet.microsoft.com/download)
- Visual Studio 2022 or VS Code (recommended)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/hoangtuan2k5/fundamental-dsa.git
cd fundamental-dsa
```

2. Restore dependencies:
```bash
dotnet restore
```

3. Build the solution:
```bash
dotnet build
```

4. Run tests:
```bash
dotnet test
```

5. Run the console application:
```bash
dotnet run --project FundamentalDSA.ConsoleApp
```

## 💡 Usage Examples

### Static Array
```csharp
var staticArray = new StaticArray<int>(10);
staticArray[0] = 42;
int value = staticArray[0];
```

### Dynamic Array
```csharp
var dynamicArray = new DynamicArray<string>();
dynamicArray.Add("Hello");
dynamicArray.Add("World");
string item = dynamicArray[0];
```

### Single Linked List
```csharp
var linkedList = new SingleLinkedList<int>();
linkedList.AddFirst(1);
linkedList.AddLast(2);
linkedList.AddLast(3);
```

### Binary Search Tree
```csharp
var bst = new BinarySearchTree<int>();
bst.Insert(50);
bst.Insert(30);
bst.Insert(70);
bool found = bst.Search(30);
```

### Hash Table with Separate Chaining
```csharp
var hashTable = new HashTableSeparateChaining<string, int>();
hashTable.Put("key1", 100);
int value = hashTable.Get("key1");
```

### Quick Sort
```csharp
int[] array = { 64, 34, 25, 12, 22, 11, 90 };
QuickSort.Sort(array);
```

## 🧪 Testing

Each data structure and algorithm includes comprehensive unit tests using xUnit framework:

```bash
# Run all tests
dotnet test

# Run tests with coverage
dotnet test --collect:"XPlat Code Coverage"
```

## 📚 Learning Resources

Each implementation includes:
- **Time Complexity Analysis**: Big O notation for operations
- **Space Complexity Analysis**: Memory usage characteristics
- **Use Cases**: When to use each data structure/algorithm
- **Trade-offs**: Advantages and disadvantages
- **Visual Examples**: ASCII diagrams where applicable

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Guidelines
- Follow C# coding conventions
- Add unit tests for new features
- Update documentation as needed
- Ensure all tests pass before submitting

## 📋 Implementation Checklist

### Data Structures
- [ ] Static Array
- [ ] Dynamic Array
- [ ] Single Linked List
- [ ] Double Linked List
- [ ] Circular Single Linked List
- [ ] Circular Double Linked List
- [ ] Stack (Array-based)
- [ ] Stack (List-based)
- [ ] Queue (Array-based)
- [ ] Queue (List-based)
- [ ] Tree
- [ ] Binary Tree
- [ ] Binary Search Tree
- [ ] AVL Tree
- [ ] Red-Black Tree
- [ ] Splay Tree
- [ ] B-Tree
- [ ] B+ Tree
- [ ] Hash Table
- [ ] Hash Functions
- [ ] Hashtable Separate Chaining
- [ ] Hashtable Open Addressing
- [ ] Hashtable Linear Probing
- [ ] Hashtable Quadratic Probing
- [ ] Hashtable Double Hashing
- [ ] Graph

### Algorithms
- [ ] Breadth-First Search
- [ ] Depth-First Search
- [ ] Uniform Cost Search
- [ ] Dynamic Programming
- [ ] Bubble Sort
- [ ] Insertion Sort
- [ ] Selection Sort
- [ ] Quick Sort
- [ ] Merge Sort
- [ ] Heap Sort
- [ ] Radix Sort

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♂️ Author

**Hoàng Chiều Nguyễn Tuấn** - [@hoangtuan2k5](https://github.com/hoangtuan2k5)

*Passionate about Data Structures, Algorithms, and Computer Science education*

## 🙏 Acknowledgments

- Inspired by classic computer science textbooks
- Built for educational purposes and learning
- Community contributions and feedback

---

⭐ Star this repository if you find it helpful for learning DSA concepts!
