# Browser History Simulator

A simple command-line program that simulates a web browser's back and forward navigation, built on a custom **Stack** data structure in Python.

## How It Works

Two stacks track your browsing history:

- **`redo` stack**: holds pages you've visited; the top is your current page.
- **`undo` stack**: holds pages you've gone back from, so you can return to them.

Moving back pops a page from `redo` onto `undo`, and moving forward does the reverse.

## Stack Operations

| Method | Description |
|--------|-------------|
| `push(e)` | Add an element to the top |
| `pop()` | Remove and return the top element |
| `top()` | Return the top element without removing it |
| `isEmpty()` | Check if the stack is empty |
| `Length()` | Return the number of elements |
| `content()` | Print the stack's contents |

## Usage

Requires Python 3.

```bash
python main.py
```

Commands (case-insensitive):

| Key | Action |
|-----|--------|
| `N` | Open a new webpage (enter its address) |
| `B` | Move back to the previous page |
| `F` | Move forward to the next page |
| `Exit` | Quit the program (asks for confirmation) |

## Example

```
enter your request
N
enter the webpage address
google.com
you are now visiting google.com

enter your request
B
There is no previously opened page. you open only:--> google.com
```

## Concepts Demonstrated

- Stack (LIFO) data structure
- Using two stacks to implement undo/redo-style navigation
- Simple CLI input loop

