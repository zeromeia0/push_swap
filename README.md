# Push_Swap - Sorting Algorithm Project

## Overview
Push_Swap is a sorting algorithm project that sorts a stack of integers using a limited set of operations. The goal is to sort the numbers in ascending order with the fewest possible operations.

## Installation
1. Clone the repository:
git clone https://github.com/your-username/push_swap.git
cd push_swap

2. Compile the program:
make

## Usage
### Basic Usage
./push_swap [list of integers]

Example:
./push_swap 3 1 4 2 5

### With String Input
You can also pass numbers as a single string:
./push_swap "3 1 4 2 5"

### Using the Checker
To verify that your sorting is correct, use the provided checker program (checker_linux):
./push_swap [numbers] | ./checker_linux [numbers]

Example:
./push_swap 3 1 4 2 5 | ./checker_linux 3 1 4 2 5

If the checker outputs "OK", your sorting was successful.

## Features
- Sorts small stacks (3 or 5 numbers) with optimized algorithms
- Handles larger stacks (100+ numbers) using radix sort
- Input validation for numbers and duplicates
- Visual feedback for operations performed

## Makefile Commands
- `make` - Compile the program
- `make clean` - Remove object files
- `make fclean` - Remove object files and executable
- `make re` - Recompile the program
- `make norm` - Check code style with norminette

## Testing
The Makefile includes several test commands:
- `make proof` - Test with random numbers and checker
- `make count_one` - Test with 100 random numbers and count operations
- `make count_two` - Test with 500 random numbers and count operations
- `make cem` - Test with 100 numbers
- `make quin` - Test with 500 numbers
- `make vcem`/`make vquin` - Valgrind tests for memory leaks

## Notes
- Only integers within the range of INT_MIN to INT_MAX are accepted
- Duplicate numbers will be rejected
- The program will exit with an error if invalid input is provided

Enjoy sorting!
