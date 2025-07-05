# 🤖 VJ Save Restricted Bot

> **A powerful Telegram bot that saves and forwards restricted content from channels and groups with advanced login features**

---

## ✨ Features

- 📋 **Save restricted content** from any Telegram channel/group
- 🔐 **Secure login system** with string session management
- 🔗 **Multiple link formats** support (public, private, bot links)
- 📦 **Bulk message forwarding** with range support
- 🎯 **Easy to use** with simple commands
- 🛡️ **Admin controls** for user management

---

## 🚀 Quick Start

### 1. Get Your Credentials

| Variable | Description | Get From |
|----------|-------------|----------|
| `API_ID` | Your Telegram API ID | [my.telegram.org](https://my.telegram.org) |
| `API_HASH` | Your Telegram API Hash | [my.telegram.org](https://my.telegram.org) |
| `BOT_TOKEN` | Your Bot Token | [@BotFather](https://telegram.me/BotFather) |
| `ADMINS` | Admin User IDs (comma-separated) | Your Telegram User ID |
| `DB_URI` | MongoDB Database URL | [MongoDB Atlas](https://mongodb.com) |
| `ERROR_MESSAGE` | Show error messages (`True`/`False`) | Set to `True` or `False` |

### 2. Get MongoDB Database
1. Go to [MongoDB Atlas](https://mongodb.com)
2. Create a free account
3. Create a new cluster
4. Get your connection string (replace `<password>` with your actual password)

---

## 🎮 Bot Commands

| Command | Description |
|---------|-------------|
| `/start` | Start the bot and check if it's working |
| `/help` | Get detailed usage instructions |
| `/login` | Login with your Telegram string session |
| `/logout` | Logout from your current session |
| `/cancel` | Cancel any ongoing operation |

---

## 📖 How to Use

### 📢 For Public Channels/Groups
Simply send the post link:
```
https://t.me/channelname/123
```

### 🔒 For Private Channels/Groups
1. First send the invite link (if not already a member):
```
https://t.me/+AbCdEfGhIjKlMnOp
```
2. Then send the post link:
```
https://t.me/c/1234567890/123
```

### 🤖 For Bot Messages
Send the link in this format:
```
https://t.me/b/botusername/123
```

### 📦 For Multiple Messages
Send links with range format:
```
https://t.me/channelname/100-110
https://t.me/c/1234567890/50 - 60
```

---

## 🌐 Deployment Options

### 🟢 Method 1: Scalingo
1. Fork this repository
2. Create account on [Scalingo](https://scalingo.com)
3. Create new app
4. Connect your GitHub repository
5. Add environment variables in Settings
6. Deploy!

### 🔵 Method 2: Back4App
1. Fork this repository
2. Create account on [Back4App](https://back4app.com)
3. Create new app
4. Connect GitHub repository
5. Set environment variables
6. Deploy container

### 🟣 Method 3: VPS/Server
```bash
# Clone repository
git clone https://github.com/UTK253/PERSONAL_SRCB
cd PERSONAL_SRCB

# Install dependencies
pip3 install -r requirements.txt

# Set environment variables
export API_ID="your_api_id"
export API_HASH="your_api_hash"
export BOT_TOKEN="your_bot_token"
export ADMINS="your_admin_id"
export DB_URI="your_mongodb_uri"
export ERROR_MESSAGE="True"

# Run the bot
python3 bot.py
```

### 🟡 Method 4: Google Colab
1. Open [Google Colab](https://colab.research.google.com)
2. Create new notebook
3. Run this code:
```python
!git clone https://github.com/UTK253/PERSONAL_SRCB
%cd PERSONAL_SRCB
!pip install -r requirements.txt

# Set your variables
import os
os.environ['API_ID'] = 'your_api_id'
os.environ['API_HASH'] = 'your_api_hash'
os.environ['BOT_TOKEN'] = 'your_bot_token'
os.environ['ADMINS'] = 'your_admin_id'
os.environ['DB_URI'] = 'your_mongodb_uri'
os.environ['ERROR_MESSAGE'] = 'True'

!python bot.py
```

### 🐳 Method 5: Docker
```bash
# Build image
docker build -t vj-save-bot .

# Run container
docker run -e API_ID="your_api_id" \
           -e API_HASH="your_api_hash" \
           -e BOT_TOKEN="your_bot_token" \
           -e ADMINS="your_admin_id" \
           -e DB_URI="your_mongodb_uri" \
           -e ERROR_MESSAGE="True" \
           vj-save-bot
```

### 🔧 Method 6: Non-Docker Local
```bash
# Install Python 3.10+
# Clone repository
git clone https://github.com/UTK253/PERSONAL_SRCB
cd PERSONAL_SRCB

# Create virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Create .env file with your variables
echo "API_ID=your_api_id" > .env
echo "API_HASH=your_api_hash" >> .env
echo "BOT_TOKEN=your_bot_token" >> .env
echo "ADMINS=your_admin_id" >> .env
echo "DB_URI=your_mongodb_uri" >> .env
echo "ERROR_MESSAGE=True" >> .env

# Run the bot
python bot.py
```

---

## ⚠️ Important Notes

- **Never share your API credentials** with anyone
- **Use environment variables** for sensitive data, don't hardcode them
- **Keep your bot token secure** and regenerate if compromised
- **MongoDB URI** should be kept private and secure
- **Test with small message ranges** before bulk forwarding

---

## 🛠️ Troubleshooting

### Common Issues:
- **Bot not responding**: Check if bot token is correct
- **Login issues**: Verify API_ID and API_HASH
- **Database errors**: Ensure MongoDB URI is correct and accessible
- **Permission errors**: Make sure the account has access to the source chat

### Getting Help:
1. Check the bot's `/help` command
2. Verify all environment variables are set correctly
3. Check bot logs for error messages
4. Ensure your account is not restricted

---

## 🏆 Credits

- **Special Thanks**: [B3ASTX BOTS](https://t.me/B3ASTX_BOTS)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## ⭐ Support

If this project helped you, please give it a ⭐ star!

**Need help?** Contact [@B3ASTX_BOTS](https://t.me/B3ASTX_BOTS)

---

<div align="center">
  <b>Made with ❤️ by the Telegram Bot Community</b>
</div>
