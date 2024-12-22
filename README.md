# MultiplayerTest

This project demonstrates a basic multiplayer setup using **Netcode for GameObjects** in Unity. The project includes functionality for hosting a game, joining as a client, synchronizing player transforms across the network, and interacting with an object.

## Features

- **Host Setup**: The game can be hosted on one machine, which acts as the server.
- **Client Join**: Other players can join as clients using the host's IP address.
- **Transform Sync**: The player’s position, rotation, and scale are synchronized across the network.
- **Interactable Object**: Players can interact with an object in the scene.

## How to Use

### 1. Build the Project

1. Open the project in Unity.
2. Build the project for your desired platform (e.g., PC).

### 2. Host a Game

- On the first PC, start the game and create a **host**. This machine will act as the **server**.
- The host will automatically start both the server and the client.

### 3. Join as a Client

- On another PC, run the game and **join** clicking the client button.
- The client will connect to the host and sync player positions.

### 4. Transform Synchronization

- The player’s **transform** (position, rotation, and scale) is synchronized across the network.
- Any movement or transformations will be reflected on all connected clients.

### 5. Interactable Object

- An object in the scene has been made **interactable**.
- Players can **interact** with this object.
- The interaction is synchronized, so other players will see the interaction in real time.

## Requirements

- **Same Network**: Both the host and client should be connected to the **same local network** (same router) for the connection to work properly.

## Troubleshooting

- **Not connecting?**: Ensure both machines are on the same local network and that you have configured **port forwarding** if playing over the internet.
- **Firewalls**: Make sure the firewall is not blocking the game’s port (usually port `7777` by default).


