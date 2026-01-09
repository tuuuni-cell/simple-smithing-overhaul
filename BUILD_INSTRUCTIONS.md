# Build Instructions for Simple Smithing Overhaul - Fabric 1.21.11

## Prerequisites
- Java Development Kit (JDK) 21 or newer
- Git installed on your system

## Step 1: Download the Source Code
```bash
git clone https://github.com/pajicadvance/simple-smithing-overhaul.git
cd simple-smithing-overhaul
```

## Step 2: Checkout the Fabric 1.21.11 Version
```bash
git checkout multicutter
```

## Step 3: Navigate to the Version Directory
```bash
cd versions/1.21.11-fabric
```

## Step 4: Build the Mod
From the root directory of the project, run:
```bash
./gradlew build
```

On Windows, use:
```bash
gradlew.bat build
```

## Step 5: Locate the Built Mod
After the build completes successfully, the mod JAR file will be located at:
```
build/libs/simple-smithing-overhaul-fabric-1.21.11.jar
```

## Step 6: Install the Mod
1. Locate your Minecraft mods folder:
   - **Windows**: `%APPDATA%\.minecraft\mods`
   - **macOS**: `~/Library/Application Support/minecraft/mods`
   - **Linux**: `~/.minecraft/mods`

2. Copy the JAR file from `build/libs/` to your mods folder

3. Make sure you have Fabric Loader installed for Minecraft 1.21.11

4. Launch Minecraft with the Fabric profile

## Notes
- The mod is now modified to remove the level 1 enchantment limit for villager trades
- You can now get higher level enchanted books from villagers (configurable via config file)
- Build time may take a few minutes depending on your system

## Troubleshooting
- If build fails, make sure Java 21+ is installed: `java -version`
- Delete the `build/` folder and try building again if you encounter caching issues
- Ensure you're in the correct git branch: `git branch` (should show `multicutter` with asterisk)
