Project Name: my-first-app
Branch: main
Install Command: npm ci  # or yarn install
Build Command: npm run build  # or yarn build
Output Directory: dist  # or build
# Ctrl Play 🎮

Ctrl Play is a hub for retro-style games built on [@aoTheComputer](https://twitter.com/aoTheComputer) and powered by [@arweaveeco](https://twitter.com/arweaveeco). This platform offers a collection of exciting games with on-chain social profiles and scores. These social profiles are built on the **Pulse Protocol**, making them reusable across any platform using Pulse.

![image](https://github.com/user-attachments/assets/76e71ce4-bf36-413f-abce-f680bb7e51d1)

---

## ✨ Features

### 🚀 Retro-Style Games
- **Games List**: Includes popular classics like *4 Cards*, *Just Slide*, *Weave Word*, *Pacman*, *Chess*, and more.
- **Interactivity**: Each game is treated as a POST on the **Pulse Protocol**, allowing users to comment and interact.

### 🧑‍🤝‍🧑 On-Chain Social Profiles
- Profiles are stored on the AO with the help of Pulse Protocol.
- Scores and activities are tied to these profiles and can be accessed across multiple platforms using Pulse.

### 💬 Social Interactions
- Users can submit posts and interact with games through the Lua backend.
- Example Lua code to submit a post:
  ```lua
  target = "E8gHiH6gpkfFZywTbQj13F9SUH8N9tWrFsgGisOPHV4"

  Send({Target = target, Action = "SUBMIT_POST", Tags = {content= "Just Slide Remastered"}})
  ```

## 🔧 Technical Details

### Frontend
- Built using React and Tailwind CSS for a modern and responsive UI.
### Backend
- Written in Lua, leveraging the Pulse Protocol for decentralized social interactions.
### Pulse Protocol
- A social graph protocol initially developed for Ctrl Play, now available for anyone to use.
- Profiles and posts are stored on-chain. 
- Website: [Pulse Protocol](https://pulseprotocol.vercel.app/)
- Docs: [Pulse Protocol Documentation](https://abhays-organization-2.gitbook.io/pulse-protocol-docs)

## 👥 Team
- [Aditya Chaudhary](https://x.com/ItsAditya_xyz) - Developer
- [Abhay Gupta](https://x.com/professorabhay) - Developer
- [Nancy Dubey](https://x.com/NancyDubey_) - Designer

## 🌐 Links
### [Twitter](https://x.com/CtrlPlayxyz)
### [Protocol Land](https://protocol.land/#/repository/0291eafa-e91d-4575-8bed-4d7c5c9043c9/)
