# Minigrep

Minigrep is a command-line utility inspired by the classic `grep` tool. It allows users to search for specific patterns within files, making it an essential tool for developers and system administrators to quickly locate and analyze text within files.

## Features

- **Case-sensitive search**: By default, Minigrep performs case-sensitive searches.
- **Case-insensitive search**: Optionally, Minigrep can perform case-insensitive searches.
- **Simple command-line interface**: Intuitive and easy-to-use interface.
- **Efficient file processing**: Handles large files efficiently.

## Installation

To install Minigrep, you'll need to have Rust installed on your system. If you don't have Rust installed, you can download it from [rust-lang.org](https://www.rust-lang.org/).

Once you have Rust installed, clone the repository and build the project:

```bash
git clone https://github.com/your-username/minigrep.git
cd minigrep
cargo build --release
```

This will create an executable in the `target/release` directory.

## Usage

To use Minigrep, you need to provide two arguments: the query string and the file path. Here is the basic syntax:

```bash
./minigrep <query> <file_path>
```

### Example

To search for the word "rust" in a file named `example.txt`, run:

```bash
./minigrep rust example.txt
```

### Case-insensitive search

To perform a case-insensitive search, set the `IGNORE_CASE` environment variable:

```bash
IGNORE_CASE=1 ./minigrep rust example.txt
```

## Project Structure

- **src**: Contains the source code for Minigrep.
  - **main.rs**: The entry point of the application.
  - **lib.rs**: Contains the core functionality of Minigrep.
- **tests**: Contains the unit tests for the project.
- **Cargo.toml**: Contains the project metadata and dependencies.

## Contributing

Contributions are welcome! If you have suggestions for improvements or find any bugs, please open an issue or submit a pull request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a new Pull Request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project is part of the "An I/O Project: Building a Command Line Program" from [The Rust Programming Language](https://doc.rust-lang.org/book/ch12-00-an-io-project.html). Special thanks to the Rust community for their valuable resources and contributions.

---

Happy coding! 🚀