# CLI Application with Picocli Subcommands

This is a small command-line interface (CLI) application built using Java and [Picocli](https://picocli.info/). The project demonstrates the use of subcommands with Picocli by providing two basic commands: `hello` and `goodbye`. The application accepts a user's name and either greets or bids farewell to them.

## Project Structure

The application consists of three main components:

1. **Main class**: The entry point of the application. It serves as the parent command and registers the subcommands.
2. **Hello command**: A subcommand that prints a personalized greeting to the user.
3. **Goodbye command**: A subcommand that prints a personalized farewell to the user.

## Requirements

- Java 11 or later
- Maven 3.6 or later

## How to Build

To build the project, follow these steps:

1. Clone this repository to your local machine:
   ```bash
   git clone <repository-url>
   ```

2. Navigate to the project's root directory:
   ```bash
   cd <project-directory>
   ```

3. Run Maven to compile and package the application:
   ```bash
   mvn clean package
   ```

This command will compile the Java classes and create an executable JAR file in the `target` directory.

## How to Run

To run the CLI application, use the following commands from your terminal:

### Run the JAR File

After building the project, an executable JAR file will be created in the `target` directory, for example:
```bash
java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar [command] [options] [name]
```

### Available Commands

- **`hello`**: Prints a greeting message.

  Example:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello John
  ```

  Output:
  ```
  Hello John!
  ```

    - You can customize the greeting message using the `--greetings` option:
      ```bash
      java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar hello --greetings "Hi there" John
      ```

      Output:
      ```
      Hi there John!
      ```

- **`goodbye`**: Prints a farewell message.

  Example:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye John
  ```

  Output:
  ```
  Goodbye John!
  ```

    - You can customize the farewell message using the `--farewells` option:
      ```bash
      java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar goodbye --farewells "See you later" John
      ```

      Output:
      ```
      See you later John!
      ```

### Additional Options

- **Help**: You can display help information by using the `--help` or `-h` option:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar --help
  ```

- **Version**: Display the version information using the `--version` or `-V` option:
  ```bash
  java -jar target/java-intellij-idea-and-maven-1.0-SNAPSHOT.jar --version
  ```
  
### About this Readme file
This file has been partly generated using ChatGPT.
