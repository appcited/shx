# shx.run

```text
                  /$$
                 | $$
         /$$$$$$$| $$$$$$$  /$$   /$$
        /$$_____/| $$__  $$|  $$ /$$/
       |  $$$$$$ | $$  \ $$ \  $$$$/
        \____  $$| $$  | $$  / $$ $$
        /$$$$$$$/| $$  | $$ / $$/\ $$
       |_______/ |__/  |__/|___/  \__/

 A minimal, customizable CLI written in shell
                   shx.run
```

## Installation

1. Copy the `shx` to your project root and make it executable.

    ```sh
    chmod +x shx
    ```

## Usage

1. Create a `run` directory in your project.

    ```sh
    mkdir run
    ```

2. Create a script for your command in the `run` directory.

    ```sh
    echo '#!/bin/sh' >> run/hello
    echo 'echo hello world!' >> run/hello
    chmod +x run/hello
    ```

3. Run your command.

    ```sh
    shx run/hello
    ```

## Convention over Configuration

Shx uses a convention over configuration approach. This means that
you can use it without any configuration, but you can also customize it to your
needs.

## Features

### Filesystem routing

Use transparent filesystem routing for shx command structures.

[Example](examples/filesystem-routing/README.md)

### Directory commands

Use commands with the same name as the directory to implement directory commands.

[Example](examples/directory-commands/README.md)

### Wildcard commands

Use wildcard paths to execute all matching commands.

[Example](examples/wildcard-commands/README.md)

### Flexible commands

Use any executable or script as building blocks for your shx commands.

[Example](examples/basic/README.md)

### Pass command arguments

Pass any arguments to the executed command.

[Example](examples/pass-command-arguments/README.md)

### Shell autocompletion

Use out-of-the-box autocompletion in all shell environments.

[Example](examples/shell-autocompletion/README.md)

### Display available commands

Use the default command to display all available commands.

[Example](examples/display-available-commands/README.md)

### Hooks

Use hooks to intercept, extend and alter command execution.

[Example](examples/hooks/README.md)
