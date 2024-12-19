# TON Shop

A Telegram bot-powered shop built with TON blockchain integration.

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/ton-shop.git
cd ton-shop
```

### 2. Create Telegram Bot

1. Open Telegram and search for [@BotFather](https://t.me/BotFather)
2. Start a chat with BotFather and send `/newbot`
3. Follow the instructions to create your bot
4. Save the API token provided by BotFather - you'll need it for the `.env` file

### 3. Configure Environment Variables

Create a `.env` file in the root directory and add the following:

```env
BOT_TOKEN=your_telegram_bot_token_here
# Add any other required environment variables
```

### 4. Build the Project

Install dependencies and build the project:

```bash
npm install
npm run build
```

### 5. Deploy to Netlify

1. Create a Netlify account if you don't have one
2. Install Netlify CLI:
   ```bash
   npm install -g netlify-cli
   ```
3. Deploy the build directory:
   ```bash
   cd build
   netlify deploy --prod
   ```
4. Follow the prompts to complete the deployment
5. Save the deployment URL - you'll need it for your bot configuration

### 6. Run the Bot

Start the Telegram bot:

```bash
node Bot/bot.js
```

## Additional Information

- Make sure you have Node.js installed (version 14 or higher recommended)
- The bot will be available at your configured Telegram handle
- The shop interface will be accessible through the Netlify deployment URL

For issues or contributions, please open an issue or PR in the repository.