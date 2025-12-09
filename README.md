# Unpack-FileServer

## Overview

This repository contains unpacked game files from the RYL (Ragnarok Online-like) MMORPG, organized as a fileserver for different server versions. The files have been extracted from game archives and are structured for easy access and modification. This project is intended for game developers, modders, and enthusiasts interested in RYL game mechanics, scripting, and asset management.

RYL is a popular MMORPG that features fantasy elements, quests, skills, and multiplayer gameplay. The unpacked files include scripts, configurations, zone data, and dynamic link libraries (DLLs) used by the game server and client.

## Project Structure

The repository is organized into three main directories, each representing a different server version or variant:

### Eternal/
- **Description**: Files for the Eternal server version.
- **Key Files**:
  - `Chemical.gsf`: Chemical-related scripts.
  - `DroneView.dll`, `FameBar.dll`, `Loader.dll`, `Neck_Cloak.dll`, `ResolutionFix.dll`: DLLs for various game functionalities (e.g., UI fixes, loaders).
  - `ItemScript.gsf`: Item definitions and scripts.
  - `MineralVein*.gsf`: Mineral vein configurations.
  - `MonsterProtoType.gsf`: Monster prototype data.
  - `NPCScript.mcf`: NPC scripts.
  - `Quest.mcf`: Quest definitions.
  - `Script.mcf`, `Script1.gsf`: General scripts.
  - `SkillScript.gsf`, `SkillScriptEx.gsf`: Skill-related scripts.
  - `SpeacialCompensation.gsf`: Special compensation data.
  - `VersionInfo.dat`: Version information.
  - `zone*.z3s`: Zone files for game maps (e.g., zone1.z3s to zone100.z3s).
- **Loader.txt**: Lists DLLs to load for this version (e.g., DroneView.dll, Famebar.dll).

### GempakZ/
- **Description**: Files for the GempakZ server version.
- **Key Files**:
  - Similar to Eternal, with some variations (e.g., `HotaiMalaysia.dll`, `nProtect.dll`).
  - `Gempakz.md`: (Currently empty; placeholder for documentation).
- **Loader.txt**: Lists DLLs to load (e.g., Neck_Cloak.dll, Famebar.dll).

### Unity/
- **Description**: Files for the Unity server version.
- **Key Files**:
  - Includes additional DLLs like `ArmorGlow.dll`, `oggs.dll`, `Proxy.dll`.
  - Zone files and scripts similar to other versions.
- **Loader.txt**: Lists DLLs to load (e.g., oggs.dll, Proxy.dll).

## File Types

- **.gsf**: Game Script Files – Contain scripts for items, skills, chemicals, etc. These are likely Lua or custom scripting language files.
- **.mcf**: Configuration Files – Used for quests, NPCs, and general scripts.
- **.z3s**: Zone Files – Define game map zones and layouts.
- **.dll**: Dynamic Link Libraries – Executable modules for game enhancements, fixes, or features (e.g., resolution fixes, UI bars).
- **.dat**: Data Files – Contain version info or other binary data.
- **.txt**: Text Files – Such as Loader.txt, which specifies DLLs to load.

## Purpose

This repository serves as a centralized fileserver for RYL game assets, allowing developers to:
- Modify game scripts for custom content.
- Analyze game mechanics and balance.
- Develop mods or private servers.
- Preserve historical game data.

**Note**: These files are unpacked from proprietary game archives. Ensure compliance with game licensing and copyright laws when using or distributing.

## Usage

1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/Unpack-FileServer.git
   cd Unpack-FileServer
   ```

2. **Integrate with Game Server/Client**:
   - Copy the relevant directory (e.g., `Eternal/`) to your RYL game server directory.
   - Load the DLLs listed in `Loader.txt` using the game's loader mechanism.
   - Edit `.gsf` and `.mcf` files using a text editor or script editor (e.g., for Lua syntax if applicable).
   - For zone files (`.z3s`), use appropriate tools to view or edit map data.

3. **Development Tips**:
   - Backup original files before modifications.
   - Test changes in a controlled environment to avoid game instability.
   - Use version control to track changes in scripts.

## Requirements

- RYL game client/server software.
- Text editor for script editing (e.g., VS Code, Notepad++).
- Basic understanding of game scripting and file structures.

## Contributing

Contributions are welcome! If you have improvements, bug fixes, or additional unpacked files:
1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request with a clear description.

Please ensure all contributions respect the original game's terms of service.

## License

This project is for educational and research purposes. The original game files are proprietary. See the game's EULA for usage rights.

## Credits

- Unpacked using custom tools (e.g., unpack tools mentioned in scripts).
- Original game: RYL MMORPG by [Game Developer/Company].
- Contributors: [Your Name/Contributors].

## Contact

For questions or support, open an issue on GitHub or contact [your email/contact info].