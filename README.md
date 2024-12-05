

# 🚀 **Solana Copy Trading Bot** 🤖  

🔗 **Powered by:** Jupiter Aggregator, Solana Web3.js, and SPL Token libraries.  

This bot monitors Jupiter swaps in real-time 🌍, replicates trades 🔄, and optimizes profits 💰 by executing trades based on predefined market conditions.  

---

## 📖 **Features**  

1. **Real-Time Monitoring** 🕒:  
   - Leverages WebSocket to track Jupiter swap transactions live.  
   - Extracts critical data like token addresses, amounts, and prices.  

2. **Smart Trade Execution** 🎯:  
   - Automatically buys or sells based on swap details.  
   - Ensures optimal SOL balance and maintains reserves.  

3. **Detailed Metadata** 📊:  
   - Fetches token metadata like name, symbol, and logo using Metaplex SDK.  
   - Calculates prices and value in USD.  

4. **Customizable** 🔧:  
   - Easily configure the target wallet, buy/sell limits, and RPC endpoints.  

5. **Analytics** 📈:  
   - Logs transaction details with swap values and links to Solscan for transparency.  

---

## 📦 **Installation**  

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/solana-copy-trading-bot.git
   cd solana-copy-trading-bot
   ```

2. Install dependencies:  
   ```bash
   npm install
   ```

3. Add your environment variables:  
   - Create a `.env` file with the following:  
     ```
     PRIVATE_KEY=<your_wallet_private_key>
     RPC_ENDPOINT=https://api.mainnet-beta.solana.com
     RPC_WEBSOCKET_ENDPOINT=wss://api.mainnet-beta.solana.com
     TARGET_WALLET=<target_wallet_public_key>
     MAXIMUM_BUY_AMOUNT=<max_amount_in_SOL>
     JUP_AGGREGATOR=<jupiter_program_id>
     ```

---

## 🚀 **Usage**  

1. Start the bot:  
   ```bash
   npm run start
   ```  

2. The bot will:  
   - Monitor Jupiter swaps and log the details.  
   - Execute trades automatically for eligible transactions.  
   - Display transaction results in the console.  

---

## 🛠 **How It Works**  

1. **Transaction Monitoring**:  
   The bot subscribes to real-time Solana transactions using WebSocket.  

2. **Data Extraction**:  
   - Fetches transaction logs to determine swap details.  
   - Fetches token metadata for better trade insights.  

3. **Trade Execution**:  
   - Buys or sells SOL or tokens based on predefined logic.  
   - Executes transactions with Jupiter’s aggregator for best prices.  

---

## ⚡ **Example Output**  

```plaintext
🚀 Swap: SOL - USDC  
💰 Amount: 2 SOL - 100 USDC  
💵 Amount in USD: 50 $ - 100 $  
🔗 Tx: https://solscan.io/tx/yourtxhash  
```

---

## 🛡 **Safety Features**  

- Ensures sufficient SOL balance before executing trades.  
- Rejects invalid swaps or unsupported tokens.  

---

## 💡 **Contributing**  

Feel free to submit PRs 🛠 or raise issues 🚨. Your contributions are always welcome!  

---

## 👨‍💻 **Author**  

👾 Developed by **g0drlc** | [Telegram](https://t.me/g0drlc)

🌟 **Happy Trading!** 🌟  
