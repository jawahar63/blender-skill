# Blender Skill for Claude Desktop (MCP Integration)

Enable Claude Desktop to control and interact with Blender through the Blender MCP Server.

## Overview

This skill file helps Claude Desktop communicate directly with Blender using the Blender MCP Server.

Once configured correctly, you can ask Claude to:

* Create 3D models
* Modify existing scenes
* Generate materials
* Animate objects
* Run Python scripts inside Blender
* Automate repetitive Blender workflows

## Prerequisites

Before using this skill, ensure the following are installed:

* Blender 5.1
* Claude Desktop
* Blender MCP Add-on
* Blender MCP Server enabled

## Installation

### 1. Install Blender 5.1

Download and install Blender 5.1 from the official Blender website.

### 2. Install the Blender MCP Add-on

Download the Blender MCP Add-on from:

https://www.blender.org/lab/mcp-server

Install the add-on inside Blender:
<img width="1448" height="345" alt="image" src="https://github.com/user-attachments/assets/b43241a7-0db9-4146-99b2-ba070422b519" />
1. Open Blender
2. Go to Blender mcp link
3. There will be button Called Drag and Drop into Blender
4. Drag and drop to Blender twice (First to add the Blender Lab repository, secondly to install the add-on)
5. Click **Install**
7. Enable the add-on

### 3. Enable Blender MCP Server

After enabling the add-on:

1. Open Blender Preferences
2. Locate the MCP Server settings
3. Enable the Blender MCP Server
4. Save Preferences

### 4. Add This Skill to Claude Desktop
<img width="1889" height="858" alt="image" src="https://github.com/user-attachments/assets/96a4f309-aa5d-4a4a-8e6b-45f4961bb4e3" />


Place this skill file into your Claude Desktop skills directory.

Restart Claude Desktop after adding the skill.

### 5. Restart Applications

Restart both:

* Blender
* Claude Desktop

This ensures the MCP connection is properly initialized.

## Connection Verification

Before starting any project, ask Claude:

```
Are you able to connect to Blender?
```

Claude should confirm that the Blender MCP connection is available.

If Claude cannot connect:

* Verify Blender is running
* Verify the MCP Server is enabled
* Verify the MCP Add-on is installed correctly
* Restart both Blender and Claude Desktop

## Recommended Workflow

1. Start Blender
2. Confirm MCP Server is enabled
3. Open Claude Desktop
4. Ask:

```
Are you connected to Blender?
```

5. Wait for successful confirmation
6. Provide your Blender task

Example:

```
Create a modern gaming desk setup with realistic materials and lighting.
```

or

```
Generate a low-poly medieval village scene.
```

or

```
Create a character animation where the character walks forward for 5 seconds.
```

## Best Results

For the highest quality output:

* Be specific with dimensions
* Mention art style
* Specify materials
* Include animation requirements
* Define camera angles if needed
* Provide reference images when available

### Good Prompt Example

```
Create a realistic wooden dining table.

Requirements:
- Oak wood material
- 2m width
- 1m depth
- Rounded edges
- PBR textures
- Studio lighting setup
```

### Better Prompt Example

```
Create a photorealistic Scandinavian-style living room.

Requirements:
- Natural oak furniture
- White walls
- Large window lighting
- Modern sofa
- Indoor plants
- Realistic materials
- Cycles render setup
- 4K quality
```

## Troubleshooting

### Claude Cannot Connect

Check:

* Blender is running
* MCP Add-on is enabled
* MCP Server is active
* Claude Desktop has been restarted
* Firewall is not blocking local communication

### Commands Not Executing

Try:

1. Restart Blender
2. Restart Claude Desktop
3. Re-enable the MCP Add-on
4. Verify MCP Server status

## Notes

* Blender must be running before Claude can interact with it.
* Always verify the connection before giving complex tasks.
* More detailed prompts generally produce better results.
* Local communication is typically faster and more reliable than cloud-based workflows.
