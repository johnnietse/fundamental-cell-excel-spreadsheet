# fundamental-cell-excel-spreadsheet-project

fundamental-cell-excel-spreadsheet-project is a lightweight spreadsheet application designed to implement core features such as cell navigation, data storage, and formula evaluation. This project was developed as part of a practical software engineering assignment, focusing on designing data structures and algorithms to manage spreadsheet content.

## Features

- **Text, Number, and Formula Support**:  
  - Enter text, numeric values, or formulas starting with `=` in cells.  
  - Formulas can reference other cells (e.g., `=A1+B2+5`).

- **Dynamic Cell Updates**:  
  - When a cell's value changes, all dependent cells update automatically.  

- **Error Handling**:  
  - Handles invalid formulas gracefully.  
  - Detects and prevents circular dependencies.

- **Editable Cell Representation**:  
  - View computed values directly in cells.  
  - Edit formulas in the top content bar.

## Functional Requirements

The application fulfills these core requirements:  
1. Navigate and modify spreadsheet cells.  
2. Store text, numbers, and formulas in memory.  
3. Evaluate formulas referencing other cells or constants.  
4. Update dependent cells dynamically when referenced cells change.  

## Non-Functional Requirements

- **Optimal Algorithms**: Implements the best achievable time complexity based on course-provided tools.  
- **Memory Management**: Ensures proper allocation and freeing of memory for dynamic structures.  
- **Maintainable Code**: Code is organized, readable, and documented for future maintenance.

## Project Structure

- **`defs.h`**: Shared type definitions.  
- **`interface.c` & `interface.h`**: Code for UI display and user interaction (pre-provided).  
- **`model.c` & `model.h`**: Core implementation of spreadsheet features.  
- **`testrunner.c` & `testrunner.h`**: Support code for running automated tests.  
- **`tests.c` & `tests.h`**: Unit tests for the spreadsheet features.

## Usage/Setup

**Before cloning the repository, change your working directory to the folder where you want the project to be saved:**

Navigate to the directory where you want to store the project:
```bash
cd /path/to/your/directory
```

1. Clone the repository:  
```bash
git clone https://github.com/johnnietse/fundamental-cell-excel-spreadsheet-project.git
cd fundamental-cell-excel-spreadsheet-project
```
2. Build the project using CMake:

- Create a build/ directory to keep the build artifacts separate:
```bash
mkdir build
cd build
```
- Run CMake to configure the project using the CMakeLists.txt file in the root directory:
```bash  
cmake ..
```
- After configuring the project, build it using:
```bash  
cmake --build .
```

## Design and Implementation
- Data Structures:
  - Cells are stored in a structured format to support efficient access and updates.
  - Formulas are parsed into components for evaluation and reconstruction.

- Algorithms:
  - Handles dependency updates with efficient traversal.
  - Detects errors (e.g., circular dependencies, invalid references) robustly.


## Testing
Comprehensive tests validate the following:
- Accurate storage and retrieval of cell contents.
- Proper formula parsing and evaluation.
- Dynamic updates for dependent cells.
- Robust error handling.

---

## 📸 Screenshot
![Fundamental-cell-excel-spreadsheet](https://github.com/user-attachments/assets/aa722b36-39ef-4b66-95c4-24ba89b1972b)
