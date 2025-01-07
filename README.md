# Food Ordering Telegram Bot

A React-based food ordering application that integrates with Telegram Bot API to provide a seamless ordering experience.

## Prerequisites

- Node.js (v14 or higher)
- pnpm or yarn
- Telegram account
- A domain/hosting for the web application

## Features

- 🍕 Interactive food menu with images and prices
- 🛒 Real-time shopping cart
- 💰 Automatic price calculation
- 🔄 Add/remove items functionality
- 📱 Telegram Web App integration
- 💫 Responsive design

## Project Structure

```
src/
  ├── Components/
  │   ├── Button/   # Reusable button component
  │   ├── Card/     # Food item display cards
  │   └── Cart/     # Shopping cart component
  ├── images/       # Food item images
  ├── db/           # Menu data
  └── App.js        # Main application logic
Bot/
  └── bot.js        # Telegram bot configuration
```

## Setup Instructions

### 1. Clone and Install

```bash
git clone https://github.com/agustinustheo/food-ordering-bot.git
cd food-ordering-bot
pnpm install
```

### 2. Create Telegram Bot

1. Message [@BotFather](https://t.me/BotFather) on Telegram
2. Send `/newbot` and follow the instructions
3. Save your bot token
4. Enable Web App settings:
   - Send `/mybots`
   - Select your bot
   - Go to Bot Settings > Web App
   - Enable Web App features

### 3. Environment Setup

Create a `.env` file in the root directory:

```env
BOT_TOKEN=your_telegram_bot_token_here
WEB_LINK=your_deployed_app_url
```

### 4. Development

Run the React application locally:
```bash
pnpm start
```

Start the Telegram bot:
```bash
node Bot/bot.js
```

### 5. Production Deployment

Build the React app:
```bash
pnpm run build
```

Deploy to your hosting service (e.g., Netlify):
```bash
netlify deploy --prod
```

## Usage

1. Start your bot in Telegram
2. Click the "web app" button that appears
3. Browse the menu and add items to cart
4. Review your cart and proceed to checkout
5. Complete the payment through Telegram

## Development Notes

- The app uses React's useState for state management
- Telegram Web App API is accessed via `window.Telegram.WebApp`
- Food items data is stored in `src/db/db.js`
- Cart calculations happen in real-time

## Troubleshooting

Common issues:
- If the web app button doesn't appear, verify your WEB_LINK in `.env`
- If images don't load, check the image paths in `db.js`
- For bot connection issues, verify your BOT_TOKEN

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is MIT licensed.
