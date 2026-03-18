# How a Complete Beginner Deployed the FootballBets Intelligent Contract on GenLayer Studio

**Author:** Abdullah (asmoabdullahofficial)  
**Date:** March 18, 2026  
**Wallet:** `0x75976D4d18cD9dE80d6Ab1425163bA753df7969d`

### Introduction
I had never written or deployed any smart contract before. This guide shows exactly how I deployed the official FootballBets example from the GenLayer boilerplate on **Testnet Bradbury** using only the browser-based GenLayer Studio.

### What is FootballBets?
A simple Intelligent Contract where anyone can:
- Create a football match bet (team1, team2, predicted winner)
- Resolve the bet using AI (it scrapes BBC and decides the real winner)
- Earn 1 point if your prediction is correct

### Step-by-Step Deployment (Exact clicks)

1. Go to [https://studio.genlayer.com/contracts](https://studio.genlayer.com/contracts)
2. Connect wallet (MetaMask) → used my wallet `0x75976D...7969d`
3. Click **New Contract** (+ icon)
4. Delete all default code
5. Paste the FootballBets code (from `/contracts/football_bets.py` in this repo)
6. Make sure the first line is correct: `# { "Depends": "py-genlayer:test" }`
7. Click **Save**
8. Leave Constructor inputs empty → Click **Deploy**
9. Confirm in MetaMask

**Deployment Transaction:**  
`0x6ca994a456248467a8b59dcf3eb7a8e5352cfba37ca317a3b90a171b6905bdd8`

**Contract Address:** `0xAEB01616f5a71b2696696be807A2242ca5BD146C`

### Testing the Contract

I created a test bet:
- game_date: `2026-03-18`
- team1: `Manchester United`
- team2: `Liverpool`
- predicted_winner: `0` (draw)

**create_bet Transaction:**  
`0xbd42c723461e40da3191d24f6f0cd4e2f964dee5625e7e2ffb9f69d3917591d9`

Then I called `get_bets` and it successfully returned my bet data.

### Screenshots
(Attach these when submitting to portal)
- Deployment success
- create_bet execution
- get_bets result showing the bet

### Conclusion
This proves that even a complete beginner can deploy an AI-powered Intelligent Contract on GenLayer in under 10 minutes.

GenLayer Studio makes it extremely easy. I highly recommend new builders start with this FootballBets example.

**Repository:** https://github.com/asmoabdullahofficial/genlayer-project-boilerplate  
**My other contribution:** FootballBets deployment (Builder category)

Feel free to fork this repo and follow the same steps!
