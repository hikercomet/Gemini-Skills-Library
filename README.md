# Gemini Skills Library

A comprehensive framework for reusable AI skills for the Gemini CLI.
This library provides modular prompts for tasks like code review, refactoring, documentation generation, translation, and analysis, now enhanced with a robust set of features for development, management, and distribution.

## Features

*   **Modular AI Skills:** Define AI prompts for various tasks using Markdown or YAML.
*   **Workflow Engine:** Chain multiple skills together to create complex automated workflows.
*   **Dynamic Skill Registration:** Automatically discover and register skills from the `skills` directory.
*   **Web User Interface (UI):** A Flask-based web application for intuitive interaction with skills and workflows.
*   **Command-Line Interface (CLI):** A dedicated CLI (`gemini_skills_cli.py` or `gs.bat`) for managing and running skills from the terminal.
*   **Automated Testing Framework:** Ensure skill reliability and prevent regressions with a built-in testing suite.
*   **Distributable Package:** Easily package and distribute the entire library for others to use.

## Installation

To install the `gemini-skills-lib` package, you can either install it directly from the generated wheel file or in editable mode for development.

### From a Wheel File

1.  Obtain the `gemini_skills_lib-0.1.0-py3-none-any.whl` file from the `dist/` directory.
2.  Open a terminal in the directory where the `.whl` file is located.
3.  Run the following command:
    ```bash
    pip install gemini_skills_lib-0.1.0-py3-none-any.whl
    ```

### For Development (Editable Mode)

1.  Navigate to the project's root directory.
2.  Run the following command:
    ```bash
    pip install -e .
    ```
    This allows changes to the source code to be immediately reflected without reinstallation.

## Usage

Once installed, you can interact with the Gemini Skills Library through its Web UI or CLI.

### Web User Interface (UI)

To start the Web UI:

```bash
gemini-skills-ui
```
Open your web browser and navigate to `http://127.0.0.1:5000`.

### Command-Line Interface (CLI)

You can use the `gemini_skills_cli.py` script directly or a convenient batch wrapper (`gs.bat`).

#### Using `gemini_skills_cli.py`

Navigate to the project's root directory and run:

```bash
python gemini_skills_cli.py list
python gemini_skills_cli.py register
python gemini_skills_cli.py run review --target tests/sample_code.py
python gemini_skills_cli.py workflow
```

#### Using the `gs.bat` Wrapper (Windows)

For easier access, a `gs.bat` wrapper is provided in the project root. To use it from any directory, add the project root (`C:\GeminiCLI\gemini-skills-lib`) to your system's `PATH` environment variable.

```bash
gs list
gs register
gs run review --target tests/sample_code.py
gs workflow
```

### Running Tests

To run the automated test suite:

```bash
gemini-skills-repl # Start the REPL
>>> test           # Type 'test' in the REPL
```
Alternatively, if you have the package installed in editable mode, you can run the tests directly from the project root:
```bash
python -m unittest discover tests
```

## Contributing

Feel free to add new skills, improve existing ones, or contribute to the framework itself.
"# Gemini-Skills-Library" 
