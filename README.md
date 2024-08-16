# Spreadsheet Formula Evaluator

This project is a simple spreadsheet-like application that allows users to input and evaluate mathematical expressions and formulas. The application processes formulas entered into cells, expanding ranges and applying functions to produce calculated results.

## Features

- **Basic Arithmetic**: Supports addition, subtraction, multiplication, and division with correct precedence handling.
- **Range Expansion**: Expands ranges in formulas (e.g., `A1:B2`) and applies functions across those ranges.
- **Spreadsheet Functions**: Includes built-in functions such as `SUM`, `AVERAGE`, `MEDIAN`, and more.
- **Dynamic Updates**: Updates the result in a cell as soon as the formula is changed.

## Built-in Functions

Here are some of the functions that can be used in the spreadsheet:

- `SUM(range)` - Calculates the sum of the numbers in the specified range.
- `AVERAGE(range)` - Calculates the average of the numbers in the range.
- `MEDIAN(range)` - Finds the median value in the range.
- `EVEN(range)` - Filters out only even numbers from the range.
- `SOMEEVEN(range)` - Returns `true` if any number in the range is even.
- `EVERYEVEN(range)` - Returns `true` if all numbers in the range are even.
- `FIRSTTWO(range)` - Returns the first two numbers in the range.
- `LASTTWO(range)` - Returns the last two numbers in the range.
- `HAS2(range)` - Returns `true` if the number 2 is present in the range.
- `INCREMENT(range)` - Increments each number in the range by 1.
- `RANDOM([x, y])` - Returns a random number between `x` and `x + y`.
- `RANGE([start, end])` - Returns a range of numbers from `start` to `end`.
- `NODUPES(range)` - Removes duplicate numbers from the range.

## How It Works

1. **Infix Evaluation**: The `infixEval` function evaluates infix expressions (e.g., `3 + 5`) and replaces them with their calculated results.
2. **High Precedence Operations**: The `highPrecedence` function ensures that multiplication and division are performed before addition and subtraction.
3. **Range and Cell Expansion**: The `evalFormula` function expands ranges and cell references, replacing them with actual values before applying any functions.
4. **Functions**: The `applyFunction` method applies the relevant spreadsheet function to the expanded cell values.

## Usage

1. **Input Formulas**: Enter a formula in a cell using the format `=FUNCTION(range)` or `=expression` (e.g., `=SUM(A1:A3)` or `=A1 + B2 * C3`).
2. **Auto Update**: The cell's value will update automatically to show the result of the formula.

### Example

If you input `=SUM(A1:A3)` into a cell and the values of `A1`, `A2`, and `A3` are `2`, `3`, and `4`, the cell will display `9`.

## Installation

To run this project locally:

1. Clone the repository to your local machine.
2. Open the `index.html` file in your browser.

## Contributing

If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are warmly welcome.

## License

This project is open-source and available under the MIT License.

