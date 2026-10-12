# FaceChat — Video + Chat UI Prototype

## What this prototype demonstrates
- The other participant's tile is the large main view.
- Your own preview stays small in the top-right corner.
- Chat remains visible beside the call on desktop and below the call on mobile.
- Chat messages can be typed and added locally.
- Camera and microphone permission buttons demonstrate local device preview/control.

## Important limitation
This is a **front-end prototype**, not a finished multi-user video calling service. The remote participant is a placeholder, and chat messages are local to this browser. Real video calls and cross-device chat require WebRTC plus a signaling server and a backend (for example, WebSocket signaling, room management, authentication, and TURN/STUN configuration).

## Run it
1. Unzip the project.
2. Open `index.html` in a browser for the chat UI demo.
3. To test camera/microphone, serve the folder through `localhost` or HTTPS (browser security requires a secure context) and grant permissions.

For a simple local server with Python installed:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

## Suggested next development milestone
Build room creation and real peer-to-peer calls with WebRTC, add a WebSocket signaling server, then persist chat messages and add user authentication.
