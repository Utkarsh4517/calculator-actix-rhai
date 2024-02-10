# Rust Calculator APIs with Actix-Web and Rhai

This project demonstrates how to create basic calculator APIs using Rust with Actix-Web framework for handling HTTP requests and Rhai scripting language for evaluating mathematical expressions.

## Setup

To run this project, ensure you have Rust installed on your system. You can install Rust by following the instructions on [rust-lang.org](https://www.rust-lang.org/tools/install).

## Dependencies

This project relies on the following dependencies:
- `actix-web`: A powerful, pragmatic, and extremely fast web framework for Rust.
- `rhai`: An embedded scripting language for Rust that is lightweight, fast, and supports custom function registration.

## Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/Utkarsh4517/calculator-actix-rhai.git
    ```

2. Navigate to the project directory:

    ```bash
    cd actix-rhai
    ```

3. Build and run the project:

    ```bash
    cargo run
    ```

4. Once the server is running, you can access the following endpoints:

    - `GET /multiply/{num1}/{num2}`: Multiply two numbers.
    - `GET /add/{num1}/{num2}`: Add two numbers.
    - `GET /divide/{num1}/{num2}`: Divide two numbers.
    - `GET /subtract/{num1}/{num2}`: Subtract two numbers.

    Replace `{num1}` and `{num2}` with the numbers you want to perform the operation on.

    Example:
    - `GET http://localhost:8080/multiply/5/3` will return `15`.
    - `GET http://localhost:8080/add/10/20` will return `30`.

## Project Structure

- `src/main.rs`: Contains the main server implementation.
- `src/multiply.rhai`, `src/add.rhai`, `src/divide.rhai`, `src/subtract.rhai`: Rhai scripts for performing multiplication, addition, division, and subtraction operations.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or create a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
