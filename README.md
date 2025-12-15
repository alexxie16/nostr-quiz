# Nostr LUD16 Finder

A simple web client that connects to a public Nostr relay, subscribes to kind 0 (user metadata) events, extracts Lightning addresses (`lud16`) from profiles, and displays them in real time.

### Features
- Connects to a reliable public relay (e.g., `wss://relay.damus.io`)
- Subscribes to all kind 0 events using NIP-01
- Parses the `content` JSON and extracts valid `lud16` addresses
- Displays each found address as `Found: user@domain.com`
- Automatically stops after collecting 21 addresses

### Live Demo
[Open the deployed web client](https://alexxie16.github.io/nostr-quiz/)  

### How to Run Locally
1. Clone the repo
2. Open `index.html` in any modern browser
3. The client will connect and start finding addresses automatically

### Tech
- Pure HTML + JavaScript (no external libraries)
- Native WebSocket API

Built as part of SEC Nostr coding challenge.


