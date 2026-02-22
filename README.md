#  PacketPortal

[![Discord](https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/64sNUSxuJh)

PacketPortal bridges your Discord server and Minecraft world, allowing staff to manage and deliver item packages to players with ease. Whether it’s for event rewards, donor perks, or staff gifts, PacketPortal makes delivery immersive and effortless.

##  Features
* **Discord-to-Game Delivery**: Manage everything from Discord without logging into Minecraft.
* **Immersive Effects**: Every delivery triggers a celebration with purple fireworks and "X" particles.
* **Role-Based Security**: Restrict command usage to specific Discord roles.
* **Validation**: Automatically rejects invalid items or offline players.

---

##  Discord Commands

| Command | Alias | Description | Example |
| :--- | :--- | :--- | :--- |
| `!package <name> <description> \| <items>` | - | Create a new package | `!package Starter diamond:2,bread:16` |
| `!package-give <name> <player>` | `!pg` | Send a package to a player | `!pg Starter Steve` |
| `!packages` | - | List all available packages | `!packages` |
| `!edit-package <name>` | `!ep` | Modify an existing package | `!ep Starter` |
| `!delete-package <name>` | - | Remove a package | `!delete-package Starter` |
| `!pp help` | - | View the help menu | `!pp help` |

### **Usage Example:**
1.  **Create:** `!package VIP netherite_ingot:1,golden_apple:5`
2.  **Deliver:** `!pg VIP Notch`
    * *Result: Notch receives the items in-game accompanied by purple fireworks and a "Challenge Complete" sound.*

---

##  In-Game Commands

| Command | Description |
| :--- | :--- |
| `/pp` | Opens the GUI to Create/Edit/Delete Packages. |
| `/pp reload` | Reloads the configuration and package files. |
| `/pp give` | Opens a GUI to Select and Send the Package To. |

---

##  Configuration
The `config.yml` allows you to link your bot and customize permissions:
* **bot-token**: Your Discord Bot Token.
* **allowed-roles**: List of Discord Role IDs permitted to use commands.
* **celebration-effects**: Toggle fireworks and particles on/off.

##  Requirements
* **Java**: 21+
* **Server**: Spigot or Paper 1.21.x
* **Discord**: A registered Bot Application
