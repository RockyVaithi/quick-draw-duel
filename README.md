# Quick Draw Duel 🤠

A fast multiplayer reflex game for 2–8 players on any phone or laptop.

**Play:** https://rockyvaithi.github.io/quick-draw-duel/

## How to play
1. One player taps **Create room** and shares the 4-letter code (or the invite link).
2. Friends enter the code and tap **Join**, from any device, anywhere.
3. The host taps **Start duel**.
4. Watch the screen. It flashes **yellow (HOLD)** to trick you. Don't tap.
5. When it turns **green (DRAW!)**, tap anywhere (or press Space) as fast as you can.
6. The fastest tap wins the round. Tapping early is a **foul** and scores nothing.
7. The first player to **5 points** wins the duel. Tap Rematch to go again.

You can also tap **Practice solo** to train your reaction time.

## How it works
- It's a single static `index.html` hosted on GitHub Pages.
- Players connect peer-to-peer over WebRTC through [PeerJS](https://peerjs.com). The host's browser runs the game and decides who wins.
- Fair on slow networks: each device times your reaction locally, from the moment *your* screen shows DRAW, so lag doesn't decide who wins.
