Sure! Here's a simple `README.md` template for your project that explains the functionality of the `nm` script.

### `README.md`:

```markdown
# `nm` - A Simple Notes Management Script

The `nm` script is a lightweight Bash-based tool for managing notes in Markdown format. It allows you to create, view, list, and search for notes stored in a specific directory. You can easily create notes with titles or dates, and the script integrates with Neovim to open and edit those notes.

## Features

- **Create a New Note**: Create a new note with a title or default to a date-based filename.
- **List Notes**: List all `.md` files in the notes directory and select one to edit using Neovim.
- **View a Note**: View a specific note in the terminal using `less`.
- **Search Notes**: Search through your notes for specific content using Telescope.
- **Directory Support**: Organize notes in subdirectories for better structure.

## Prerequisites

- **Bash**: The script is written in Bash, so it should work on most Unix-based systems.
- **Neovim**: Used to open and edit notes. The script assumes that Neovim is your default text editor.
- **Telescope**: The script uses the Telescope plugin for Neovim to list and search for files.
- **Packages**: FZF, Ripgrep


## Installation

1. Clone the repository or download the `nm` script to a directory on your system.
2. Ensure that Neovim and the Telescope plugin are installed.

```bash
git clone https://github.com/yourusername/nm.git
cd nm
```

3. Make the script executable:

```bash
chmod +x nm
```

4. Optionally, move the script to a directory in your `$PATH` for easy access.

```bash
mv nm /usr/local/bin/nm
```

## Usage

Run the `nm` script with the following commands:

### Create a New Note

```bash
nm new "Note Title" [subdirectory]
```

- Create a new note in the main directory or a specified subdirectory.
- If no title is provided, the script defaults to the current date as the filename.

### List All Notes

```bash
nm list
```

- List all `.md` files in the notes directory.
- Select a file to edit it with Neovim.

### View a Specific Note

```bash
nm view <filename> [subdirectory]
```

- View a specific note using the `less` command.
- Optionally, specify a subdirectory.

### Search Notes

```bash
nm search
```

- Search through all notes using the Telescope plugin for Neovim.
- This allows for fast, interactive content search within your notes.

### Example

Create a new note titled "Meeting Notes":

```bash
nm new "Meeting Notes"
```

List all available notes:

```bash
nm list
```

Search for a term in your notes:

```bash
nm search
```

## Contributing

Feel free to submit issues or pull requests if you'd like to contribute to this project. Any improvements or suggestions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```

### Explanation:
- **Features**: Describes the core features of the script.
- **Prerequisites**: Lists what is needed for the script to work (Bash, Neovim, Telescope).
- **Installation**: Provides clear instructions for setting up the script.
- **Usage**: Gives examples of the available commands (`new`, `list`, `view`, `search`).
- **Contributing**: Encourages users to contribute.
- **License**: Adds a standard open-source license section.

Feel free to adjust the instructions or descriptions to better match the exact behavior and goals of your script! Let me know if you need any further changes or additions.
