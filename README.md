# Factorio Command Center

**Factorio Command Center** is a comprehensive, web-based management interface for Factorio servers. It allows server administrators to monitor, control, and maintain their game servers with ease, whether they are running locally or hosted remotely.

## Features

- **Server Management**: Start, stop, and restart your Factorio server with a single click.
- **Real-time Monitoring**: Keep track of server status, player count, and game time.
- **Player Management**:
  - View all connected players.
  - Kick or ban players directly from the interface.
  - Send in-game messages to players.
- **Console Access**: Interact with the server console to execute commands and monitor logs.
- **File Management**: Browse and manage server files (maps, mods, saves) through a built-in file explorer.
- **Performance Metrics**: Monitor CPU and memory usage of the server process.
- **User Authentication**: Secure login system to protect your server controls.

## Prerequisites

- **Python 3.8+**
- **Factorio Server**: Ensure you have a Factorio server installed and configured.

## Installation

1.  **Clone the repository** (or download the source code).

2.  **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Configuration

Before running the application, you need to configure your Factorio server settings.

1.  **Create a configuration file** (e.g., `config.json`) or edit the default settings in the application.
2.  **Configure the following parameters**:
    - `server_path`: Path to the Factorio server executable.
    - `server_data_path`: Path to the server data directory.
    - `server_username`: Username for server authentication.
    - `server_password`: Password for server authentication.
    - `server_port`: Port number for the server (default: 33333).

## Usage

1.  **Run the application**:
    ```bash
    python app.py
    ```

2.  **Access the Web Interface**:
    Open your web browser and navigate to `http://localhost:5000` (or the port specified in the configuration).

3.  **Login**:
    Use the credentials you configured to log in.

4.  **Manage your server**:
    Use the dashboard to control your server and monitor your game.

## Project Structure

```
factorio_command_center/
├── app.py                  # Main application entry point
├── config.py               # Configuration management
├── server_manager.py       # Server process management
├── player_manager.py       # Player management logic
├── file_manager.py         # File system operations
├── templates/              # HTML templates for the web interface
│   ├── index.html
│   ├── login.html
│   ├── dashboard.html
│   └── ...
├── static/                 # Static assets (CSS, JS, Images)
├── requirements.txt        # Project dependencies
└── README.md               # This file
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
