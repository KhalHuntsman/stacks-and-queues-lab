# Stacks and Queues Lab

### Overview

This project demonstrates the implementation of **custom stack and queue data structures** in Python.  
It reinforces core data structure concepts such as **LIFO (Last In, First Out)** and **FIFO (First In, First Out)** through practical, test-driven exercises.

The lab includes:
- A queue system that simulates customer processing and winner selection
- A stack-based solution for validating balanced parentheses
- Unit tests that verify correctness and edge-case handling

This project focuses on **data structure behavior**, not performance optimizations.

### Features

- Custom Queue class with enqueue, dequeue, peek, and empty checks
- Random winner selection with controlled dequeue behavior
- Stack-based parentheses validation
- Defensive handling of empty data structures
- Fully tested using Pytest and unittest

### Queue Behavior

The custom `Queue` class supports:

- `enqueue(item)` — add an item to the end of the queue
- `dequeue()` — remove and return the front item
- `peek()` — inspect the front item without removing it
- `is_empty()` — check if the queue is empty
- `select_and_announce_winner()` — randomly selects a customer and removes all customers up to and including the winner

The queue follows **FIFO semantics**.

### Stack Behavior

The stack logic is implemented through the function:

- `is_valid_parentheses(s: str) -> bool`

This function:
- Uses a stack to track opening brackets
- Ensures parentheses are balanced and properly nested
- Supports `()`, `{}`, and `[]`
- Returns `True` only if the entire string is valid

### Technologies & Tools Used

#### Language
- Python 3

#### Testing
- Pytest
- unittest

#### Tooling
- Git & GitHub

### File Structure

All paths are listed relative to the project root.

- stacks-and-queues-lab/custom_queue.py
- stacks-and-queues-lab/custom_stack.py
- stacks-and-queues-lab/test_structures.py
- stacks-and-queues-lab/README.md

### Key Files Explained

#### custom_queue.py
- Defines a Queue class using a list-based implementation
- Implements FIFO behavior
- Includes a random winner selection feature that dequeues items correctly

#### custom_stack.py
- Implements stack logic for validating balanced parentheses
- Uses a list as a stack to track opening symbols

#### test_structures.py
- Contains unit tests for both queue and stack functionality
- Verifies correct behavior, edge cases, and return values

### Testing Notes
- Tests validate both normal and edge-case behavior
- Queue and stack logic are tested independently
- No external dependencies are required

Run tests with:
- pytest

### License
Educational use only.  
Intended for learning fundamental stack and queue data structures in Python.

### Additional notes:
- Project passed through ChatGPT for syntax and grammatical error checking and for writing this README.md. Everything was double checked for accuracy and readability prior to submission.