# Corner Grocer Data Viewer

## Overview

**Corner Grocer Data Viewer** is a command-line C++ application developed for CS-210, designed to efficiently manage and interact with grocery item data. The program reads a list of grocery items, tracks their frequencies, provides search and display functionalities, and outputs the data in both numerical and histogram formats.

## Features

- **Data Input & Processing**: Reads a plain text input file (`CS210 Project Three Input File.txt`) of grocery items, counts occurrences, and stores results in a map structure.
- **Backup Generation**: Automatically creates a backup file (`frequency.dat`) containing all input entries.
- **Interactive Menu**: Provides a console-based menu interface for:
  - Searching for specific items (with basic input sanitization and suggestions),
  - Displaying all items with occurrence counts,
  - Rendering a simple text-based histogram,
  - Exiting the program.

## File Structure

- `Project Three CS210.cpp` – Entry point; handles input validation and menu loop.
- `DataHandler.h / DataHandler.cpp` – Handles reading input, storing data in memory, and writing backups.
- `MainMenu.h / MainMenu.cpp` – Manages user interface and menu-driven operations.

## Tools and Methods

The project uses standard C++ libraries including `<map>`, `<vector>`, `<fstream>`, and `<iostream>`. Some notable implementation techniques include:

- Use of `std::map<std::string, int>` for frequency mapping.
- Input sanitation and case normalization for search accuracy.
- Defensive programming for input validation and error handling.
- Custom formatting functions for menu display aesthetics.

## Example Input

Example data format (from `CS210 Project Three Input File.txt`):
```
Broccoli
Peas
Cranberries
...
```

## Compilation

To compile and run the project:

```bash
g++ Project\ Three\ CS210.cpp MainMenu.cpp DataHandler.cpp -o GroceryViewer
./GroceryViewer
```

## Author

Dennis Ward  
CS-210 | Project Three
