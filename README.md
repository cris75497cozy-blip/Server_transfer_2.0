# Server_transfer_2.0
A Minecraft server plugin which lets you transfer players on normal aternos server or from any server FREE 1.21.11 no proxy needed 
Server_transfer_2.0
A safe, player‑controlled server‑transfer system for Paper/Spigot 1.21.1.
Designed for ARG events, multi‑server setups, and guided server transitions.
Players can only transfer themselves, and admins control all configuration.

📌 Overview
Server_transfer_2.0 provides a clean, predictable way to move players between Minecraft servers without needing a proxy like Velocity or BungeeCord. Transfers are player‑specific, meaning:

Only the player who runs a transfer command can move

No player can force another player to switch servers

Admins can configure targets through commands or config files

This makes the plugin ideal for ARG events, story servers, hub → world transitions, and controlled server switching.

✨ Features
Configurable welcome message on join

Player‑specific transfer queue

Commands like /horror and /lobby for direct transfers

/start to confirm and complete a transfer

Admin commands to add/update transfer targets

Full config reload without restarting

Alias‑based transfer system

Safe, predictable behavior

Works on Minecraft 1.21.1

🆕 New in v2.0
transfer <name> — generic alias‑based transfer

transferlist — list all configured transfers

status — show pending transfer

cancel — cancel pending transfer

transferhelp — help menu

reloadtransfer — reload config

setwelcome <message> — update join message

settarget <command> <description> <host> <port> — add/update transfer targets

Configurable join message

Admin‑only permissions for all setup commands

🧭 How It Works
Player joins → sees welcome message

Player runs a transfer command (e.g., /horror)

Plugin shows the description and queues the transfer

Player runs /start to confirm

Player is transferred to the configured host + port

Only the player who typed the command can transfer.
🧩 Commands
Player Commands

| Command | Description |
| --- | --- |
| ``/horror`` | Queue transfer to the “horror” server |
| ``/lobby`` | Queue transfer to the lobby server |
| ``/transfer ``<name>`` | Queue transfer using an alias |
| ``/start`` | Complete the queued transfer |
| ``/status`` | Show your pending transfer |
| ``/cancel`` | Cancel your pending transfer |
| ``/transferlist`` | List all transfer aliases |
| ``/transferhelp`` | Show help |
Admin Commands
| Command | Description |
| --- | --- |
| ``/settarget ``<command> ``<description> ``<host> ``<port>`` | Add/update a transfer target |
| ``/setwelcome ``<message>`` | Update join message |
| ``/reloadtransfer`` | Reload config |
🔒 Permissions
| Permission | Description |
| --- | --- |
| ``transfer.admin`` | Allows use of all admin commands |
| ``transfer.settarget`` | Allows ``/settarget`` |
| ``transfer.setwelcome`` | Allows ``/setwelcome`` |
| ``transfer.reload`` | Allows ``/reloadtransfer`` |
Player commands require no permissions.




📥 Installation
Download the latest .jar we delete older versions THIS IS 1.21.11

Drop it into your plugins folder

Start the server

Edit useing admin commands

Reload with /reloadtransfer if needed
📜 Version History
v2.0
Added alias‑based transfer system

Added /transferlist, /status, /cancel, /transferhelp

Added /setwelcome and /reloadtransfer

Improved safety and clarity

Fixed multiple transfer queue bugs

Improved join message handling

v1.0
Initial release

Basic transfer commands

/start confirmation system
🤝 Contributing
Feel free to open Issues for:

Bug reports

Feature requests

Questions

Improvements

Pull requests are welcome.
