# Rust Actix Web Project

This is a simple Rust web application built using the Actix web framework. It provides endpoints to manage a list of persons, demonstrating routing, JSON serialization, and error handling.

## Prerequisites

Before running this project, make sure you have the following installed:

- [Rust](https://www.rust-lang.org/learn/get-started)
- [Cargo](https://doc.rust-lang.org/cargo/getting-started/installation.html)

## Getting Started

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/FatGuyy/rust-Actix-restApi
   cd rust-actix-web-project
   ```

2. Compile and run the Rust application:

   ```bash
   cargo run
   ```

   The Actix web server will start, and you can access the endpoints in your browser.

## Usage

### Endpoints

- **List Persons**: Access a JSON list of persons.

  ```
  http://127.0.0.1:8080/person
  ```

- **Redirect to List Persons**: Accessing `/person/` redirects to `/person`.

  ```
  http://127.0.0.1:8080/person/
  ```

- **Get Person by ID**: Fetch a person by their ID.

  ```
  http://127.0.0.1:8080/person/{id}
  ```

### Example Usage

- Access the list of persons:
  - [http://127.0.0.1:8080/person](http://127.0.0.1:8080/person)

- Redirect to the list of persons:
  - [http://127.0.0.1:8080/person/](http://127.0.0.1:8080/person/)

- Fetch a person by ID (replace `{id}` with a valid ID):
  - [http://127.0.0.1:8080/person/1](http://127.0.0.1:8080/person/1)

## Project Structure

- `src/main.rs`: The entry point of the application, where the Actix web server is configured.

- `src/person.rs`: Contains the `Person` struct definition and implementations of the `Serialize` and `Display` traits.

## Contributing

If you'd like to contribute to this project, please follow the typical GitHub workflow:

1. Fork the repository.

2. Create a new branch for your feature or bug fix: `git checkout -b feature-name`.

3. Make your changes and commit them: `git commit -m "Description of changes"`.

4. Push your changes to your fork: `git push origin feature-name`.

5. Create a pull request to submit your changes for review.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
