# Minishell

Minishell is a custom implementation of a simple command-line shell for Unix-like operating systems. The project aims to reproduce basic shell behavior with support for running commands, environment manipulation, and error management, as part of the 42 School curriculum.

## Features

- Executes simple and compound commands
- Handles pipes (`|`) and redirections (`>`, `<`)
- Supports built-in commands (`cd`, `echo`, `env`, `exit`, etc.)
- Environment variable expansion
- Signal handling (e.g. `Ctrl+C`, `Ctrl+\`)
- Error reporting with informative messages

## Installation

Clone this repository and build the project using `make`:
```sh
git clone https://github.com/ArtPetoyan/Minishell.git
cd Minishell
make
```

## Usage

Run the shell executable:
```sh
./minishell
```
You'll be presented with a prompt. Enter commands as you would in a typical shell, e.g.:
```
minishell$ ls -la | grep Minishell > out.txt
minishell$ export MYVAR=hello
minishell$ echo $MYVAR
minishell$ exit
```

## Requirements

- Unix-like OS (Linux, macOS)
- GCC compiler
- Make utility

## Project Structure

- `src/` - Core source files for shell implementation
- `include/` - Header files
- `Makefile` - Build configuration

## Contributing

Feel free to submit issues or pull requests! Contributions to improve performance, add features, or refactor code are welcome.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgements

Made as part of the 42 Network curriculum. Thanks to everyone contributing to shell programming resources.
