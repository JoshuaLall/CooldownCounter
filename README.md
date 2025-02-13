CooldownCounter - A Minecraft Forge Mod
CooldownCounter is a Minecraft Forge mod that tracks and displays item cooldowns using a HUD overlay. It listens for specific in-game chat messages to detect when an item procs and starts a 5-minute cooldown timer, displaying the remaining time in the top-right corner of the screen.

Features

- Real-time HUD Cooldown Timer – Displays cooldown in MM:SS format.

- Chat Message Detection – Triggers cooldown when a specific message appears in chat.

- Secure License Validation – Uses HWID-based authentication to bind licenses to a single machine.

- Multiplayer Support 

How It Works
The mod listens for the message: "You have received 1x" to detect when the item procs.
Starts a 5-minute countdown (cooldownEnd = LocalDateTime.now().plusMinutes(5)).
Renders a cooldown timer in the top-right of the screen.
The timer disappears once the cooldown ends.
License validation is done via a remote server, using an HWID-based check.
