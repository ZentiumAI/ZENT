# Zentium AI

Welcome to **Zentium AI** — an innovative platform where artificial intelligence meets human ingenuity. Zentium AI combines adaptive AI agent interactions, cryptographic rewards, and collaborative problem-solving to create a unique and engaging ecosystem. Solve challenges, uncover secrets, and earn digital rewards while shaping the future of AI-driven collaboration.

---

## Key Features 🔑

### 🤖 AI Agent Interaction  
At the heart of Zentium AI are adaptive, intelligent agents. These agents guide users through intricate challenges, learning and evolving to provide personalized insights. By engaging with these agents, users uncover hidden paths, solve mysteries, and unlock digital rewards.

### 🎯 Reward System  
Participation is rewarded! Zentium incentivizes engagement with crypto rewards for solving tasks, reaching milestones, and uncovering secrets. Each interaction is meaningful, with tangible benefits for your efforts.

### 🌐 Collaborative Problem-Solving  
Some challenges require teamwork. Zentium fosters collaboration by enabling participants to join forces, share skills, and collectively overcome complex problems. Together, users and AI agents create innovative solutions that highlight the power of collective intelligence.

---

## How Zentium AI Works 🚀

1. **Interact with AI Agents**: Begin your journey by interacting with Zentium's AI agents, designed to provide tailored guidance for each user.  
2. **Solve Mysteries**: Tackle engaging challenges, uncover hidden secrets, and achieve milestones to earn rewards.  
3. **Collaborate with the Community**: Join forces with other users to solve collaborative challenges that require diverse skills and perspectives.  
4. **Earn Crypto Rewards**: Your journey is rewarded with Zentium AI’s native token `$ZENT`.  

---

## Zentium Token ($ZENT) 💎  

The native token `$ZENT` powers the Zentium AI ecosystem:  

- **Rewards**: Earn `$ZENT` for solving challenges and uncovering secrets.  
- **Governance**: Participate in decentralized governance to shape the future of the platform.  
- **Utility**: Use `$ZENT` to unlock advanced features and exclusive challenges.

---

## Installation & Setup 📦

Follow these steps to explore the Zentium AI platform:

### Prerequisites  

Make sure you have the following installed:  
- Node.js (v16+)
- Python (v3.8+)
- Git

### Use the Starter (Recommended)

```bash
git clone (https://github.com/zentium-ai/zentium-ai.git)
cd Zentium-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Once the agent is running, you should see the message to run "pnpm start:client" at the end.
Open another terminal and move to same directory and then run below command and follow the URL to chat to your agent.

```bash
pnpm start:client
```


### Manually Start Zentium (Only recommended if you know what you are doing)

```bash
# Clone the repository
git clone (https://github.com/zentium-ai/zentium-ai.git)

# Checkout the latest release
# This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
```

### Start Zentium with Gitpod


### Edit the .env file

Copy .env.example to .env and fill in the appropriate values.

```
cp .env.example .env
```

Note: .env is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON
Note: .env is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON

### Automatically Start Zentium

This will run everything to set up the project and start the bot with the default character.

```bash
sh scripts/start.sh
```

### Edit the character file

1. Open `packages/core/src/defaultCharacter.ts` to modify the default character. Uncomment and edit.

2. To load custom characters:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Multiple character files can be loaded simultaneously
3. Connect with X (Twitter)
    - change `"clients": []` to `"clients": ["twitter"]` in the character file to connect with X

### Manually Start Zentium

```bash
pnpm i
pnpm build
pnpm start

# The project iterates fast, sometimes you need to clean the project if you are coming back to the project
pnpm clean
```

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:

```
pnpm install --include=optional sharp
```
