# NeuroLedger (NL) Framework

![NeuroLedger Logo](https://gray-persistent-krill-260.mypinata.cloud/ipfs/bafybeia3wgyli7nxny2u43z6nxhhg3ujn3bkydivqdobygtesohsi5rtgu)

## Overview

NeuroLedger (NL) Framework enables real-time monitoring and analysis of Solana blockchain activity using AI-powered agents. Each agent provides unique insights and perspectives on blockchain events.

## 🤖 Default Agents

- **NeuroBit**: Blockchain & Smart Contracts specialist
- **PixelMint**: NFT & Digital Art expert
- **SolForge**: Solana Development analyst
- **TokenAlpha**: DeFi & Tokenomics advisor

## 🚀 Quick Start

### Prerequisites

- Node.js (v16 or higher)
- npm
- Internet connection

### Installation

```bash
git clone https://github.com/neuroledger/neuroledger-fw-v1.git
cd neuroledger-fw-v1
npm install
```

### Configuration

Create a `.env` file in the root directory:

```env
API_URL=https://theneuroledger.app
```

## 📋 Available Commands

### 1. List Available Agents

View all configured AI agents and their personalities:

```bash
npm run list-agents
```

### 2. Monitor New Token Creations

Watch for new token creations with AI commentary:

```bash
npm run watch-tokens <agent-name>

# Example:
npm run watch-tokens TokenAlpha
```

### 3. Monitor Token Trading Activity

Track specific token trades with AI insights:

```bash
npm run watch-token-trades <agent-name> <token-address>

# Example:
npm run watch-token-trades NeuroBit SOL_TOKEN_ADDRESS
```

### 4. Monitor Account Trading Activity

Track account-specific trading with AI analysis:

```bash
npm run watch-account-trades <agent-name> <account-address>

# Example:
npm run watch-account-trades SolForge WALLET_ADDRESS
```

### 5. Monitor Raydium Liquidity Events

Track liquidity pool activities with AI commentary:

```bash
npm run watch-liquidity <agent-name>

# Example:
npm run watch-liquidity PixelMint
```

### 6. Agent Interaction

Engage in direct conversation with an agent:

```bash
npm run agent-talk <agent-name>

# Example:
npm run agent-talk NeuroBit
```

## 🔍 Output Format

Each monitoring command provides:

- AI agent commentary
- Timestamp information
- Relevant blockchain data
- Formatted JSON output

Example output:

```json
{
  "analysis": {
    "agent": "PixelMint",
    "commentary": "Fascinating movement! This token is showing strong accumulation patterns...",
    "timestamp": "2024-01-20 15:30:45"
  },
  "data": {
    "token": "SOL",
    "action": "buy",
    "amount": "1000",
    "price": "100.50"
  }
}
```

## ⚡ Features

- Real-time blockchain monitoring
- AI-enhanced analysis
- Rate-limited API calls (2-second cooldown)
- Multiple monitoring modes
- Clean data presentation
- Graceful error handling

## 🛠 Technical Details

### Dependencies

- WebSocket for real-time data
- TypeScript for type safety
- Express for API endpoints

### Rate Limiting

- 2-second cooldown between AI analyses
- Prevents API spam
- Maintains performance

## 🤝 Error Handling

The framework handles:

- Network disconnections
- Invalid agent names
- API rate limits
- Malformed data
- Connection timeouts

## 📝 Notes

- All timestamps are in local time
- Data updates in real-time
- AI responses are rate-limited
- Ctrl+C for graceful shutdown
- Requires active internet connection

## 🔐 Security

- Keep your API keys secure
- Monitor API usage
- Use environment variables
- Don't share agent outputs publicly

## 📚 Support

For issues or questions:

1. Check error messages
2. Verify .env configuration
3. Confirm agent availability
4. Check network connection
5. Verify input parameters

## 📄 License

MIT License - See LICENSE file for details
