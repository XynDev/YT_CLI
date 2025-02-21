

# YT_CLI User Guide

**YT_CLI** is an interactive command-line tool designed to download YouTube audio in MP3 or WAV format. It also lets you manage download paths directly from the terminal using an intuitive menu.

## Prerequisites

- **FFmpeg**: YT_CLI requires [FFmpeg](https://ffmpeg.org/download.html) for audio conversion. Download and install it following the instructions from the official site.

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/XynDev/YT_CLI.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd YT_CLI
   ```

3. **Install Dependencies**:
   ```bash
   npm install
   ```

4. **Link the Package Locally** (optional but recommended):
   ```bash
   npm link
   ```
   This allows you to run `yt` globally from any terminal.

---

## Usage

### Running the Application

If you’ve linked the tool:

```bash
yt
```

If you haven’t linked the tool:

```bash
node bin/yt.js
```

### Interactive Menu Options

Once you run the command, an interactive menu will appear:

- 🎧 **Download as MP3** – Download YouTube audio in MP3 format.
- 🎙️ **Download as WAV** – Download YouTube audio in WAV format.
- 📁 **Change Download Path** – Set a custom folder for saving downloads.
- 🔄 **Restore Default Path** – Reset the download path to the default location.
- ❌ **Exit** – Close the program.

Use the arrow keys to navigate the menu and `Enter` to select an option.

---

### Example Workflow

1. Run the `yt` command.
2. Select **Download as MP3**.
3. Paste the YouTube video link when prompted.
4. Choose or confirm the download path.
5. The audio will be downloaded and converted automatically.

---

## Script Details

The main script is located in the `bin` directory:

- **yt.js**: Manages the interactive interface and handles audio download and conversion processes.
