# ECHO — The Last Signal

A first playable, local multiplayer version of the game. It uses a small Node.js HTTP server and browser polling; there are no package downloads or paid services.

## Run it

1. Open PowerShell in this folder.
2. Run `node server.js` (or `npm start`).
3. Open http://localhost:4174 in your browser.
4. To simulate a crew, open two more separate browser profiles or private windows and join with the room code. Three players are required.
5. Stop the server with Ctrl+C.

For another device on the same Wi-Fi, use the host computer's local network IP address with `:4174` (for example, `http://192.168.1.25:4174`). Windows Firewall may ask to allow Node.js on your private network. Only allow it on a trusted private network. This local version is not available to players over the public internet.

## What is included

Room creation and joining, lobby presence and leave action, 3–8 players, private roles and clues, a two-minute discussion timer, host-only shared answer submission, secret votes and public tally, three rounds, scoring, results, rematch, and responsive styling.

Rooms live in server memory and will be lost when the server stops. Reconnecting works while that process remains alive if the browser retains its room session. There is no durable storage or automatic reconnect/reassignment after someone leaves. Keep the host browser open during a game. The local server is suitable for testing on a trusted network, not public deployment.


