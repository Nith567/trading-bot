# Telegram Trading Bot

## Set Up

1. Clone this repository:

```bash
git clone https://github.com/Nith567/trading-bot.git
```

2. Provision a [CDP API Key](https://docs.cdp.coinbase.com/developer-platform/docs/cdp-keys).
3. Provision a [Telegram Bot Token](https://core.telegram.org/bots/tutorial) and register your Bot.
4. Generate a 32-byte encryption key using OpenSSL:

```bash
openssl rand -hex 32 # Save the output to use as the encryption key in Step 5.
```

5. Set the following environment variables in a `.env` file in this directory:

```bash
TELEGRAM_BOT_TOKEN="Your Telegram Bot Token"
COINBASE_API_KEY_NAME="Your CDP API Key Name"
COINBASE_API_KEY_SECRET="Your CDP API Key Private Key"
ENCRYPTION_KEY="Your hex-encoded encryption key"
```

6. Run the project:

```
npm install
npm run start
```

7. Send the `/start` message to the Bot you provisioned in Step 3 on Telegrma, and start trading!
