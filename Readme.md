# OCaml-Based Lexical Analyzer

## Project Overview

This project involves the design and implementation of a lexical analyzer using OCaml. The lexical analyzer is a crucial component in the compilation process, responsible for dividing source code into tokens that can be further processed by a compiler or interpreter.

## Features

- **Tokenization**: The analyzer divides the input text into discrete tokens. These tokens include operators, keywords, punctuation symbols, integer literals, identifiers, and unknown tokens.
- **Categorization**: Each token is categorized based on its type, such as keyword, operator, punctuation symbol, integer literal, identifier, or unknown.
- **Printing**: The tokens are organized and printed to the standard output, with each token shown along with its associated category.

## Process Steps

1. **Tokenization**: The input text is divided into individual tokens.
2. **Categorization**: Tokens are classified into their respective categories.
3. **Printing**: The categorized tokens are printed to the standard output.

## Key Functions

- **is_alnum**: Detects if a given character is alphanumeric, aiding in identifying keywords and identifiers.
- **is_punctuation**: Identifies if a character is a punctuation symbol.
- **tokenize**: The core function that receives a string as input and separates it into tokens according to specified criteria. It handles operators, punctuation symbols, whitespace, and alphanumeric characters using secondary functions. It also attempts to use exception handling to convert alphanumeric substrings into integer literals.
- **print_tokens**: Prints each token along with its category by looping over the list of tokens.
- **main**: Prompts the user to enter a string to be tokenized, reads the input string, utilizes the tokenize function, and prints the generated tokens using print_tokens.

## Prerequisites

- Ensure OCaml is installed on your system. Here we are using a VM with preinstalled OCaml.

## Setup Instructions

1. **Download or Copy Code**:
   Download or copy the code from `Lexical_Analyser.ml`.

2. **Open Terminal/CMD**:
   Open a terminal window (Linux).

3. **Navigate to Directory**:
   Use `cd` to navigate to the directory containing `Lexical_Analyser.ml`.

4. **Compile Code**:
   Compile the code using `ocamlopt` or `ocamlc`:
   ```sh
   ocamlopt -o lexical_analyzer Lexical_Analyser.ml
