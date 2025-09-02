# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2025-09-02

### Added
- Initial project setup with .NET 8.0 solution structure
- Created 4 projects architecture:
  - **FundamentalDSA.Core**: Core data structures library
  - **FundamentalDSA.Examples**: Examples and demonstrations
  - **FundamentalDSA.Tests**: Unit tests with xUnit framework
  - **FundamentalDSA.ConsoleApp**: Console application for running examples
- Comprehensive README.md with complete DSA roadmap including:
  - Arrays (Static and Dynamic)
  - Linked Lists (Single, Double, Circular variants)
  - Stacks and Queues (Array and List based)
  - Trees (Binary, BST, AVL, Red-Black, Splay, B-Tree, B+ Tree)
  - Hash Tables with collision resolution techniques
  - Graphs with search algorithms
  - Sorting algorithms (Bubble, Insertion, Selection, Quick, Merge, Heap, Radix)
  - Dynamic Programming
- Complete .gitignore file for .NET projects
- Project badges and author information
- Implementation checklist for tracking progress

### Project Structure
```
FundamentalDSA/
├── FundamentalDSA.Core/           # Core implementations
├── FundamentalDSA.Examples/       # Usage examples
├── FundamentalDSA.Tests/          # Unit tests
├── FundamentalDSA.ConsoleApp/     # Console demos
├── README.md                      # Project documentation
├── CHANGELOG.md                   # This file
├── .gitignore                     # Git ignore rules
└── FundamentalDSA.sln            # Solution file
```

### Technical Details
- Target Framework: .NET 8.0
- Testing Framework: xUnit
- Author: Hoàng Chiều Nguyễn Tuấn
- License: MIT

### Future Plans
- Implementation of all planned data structures
- Comprehensive unit tests for each component
- Performance benchmarks
- Visual examples and demonstrations
- Documentation with complexity analysis

---

## Notes

This changelog will be updated as new features and data structures are implemented. Each major milestone will be documented with detailed information about additions, changes, and improvements.
