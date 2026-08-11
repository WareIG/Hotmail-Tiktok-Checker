# Hotmail TikTok Checker

> **Created by:** @P_N_M  
> **Channel:** [@dev_raven](https://t.me/dev_raven)

A powerful tool for checking Hotmail/Outlook account validity and detecting linked TikTok, Facebook, and Instagram accounts.

## Features

- ✅ Check Microsoft/Hotmail account validity
- ✅ Detect 2FA-enabled accounts
- ✅ Identify TikTok accounts linked to emails
- ✅ Fetch TikTok profile data (followers, following, likes, videos)
- ✅ Detect linked services (TikTok, Facebook, Instagram)
- ✅ Multi-threaded for high performance
- ✅ Live progress display with colorful UI
- ✅ Auto-save hits by follower count ranges

## Preview

██████╗ █████╗ ██╗ ██╗███████╗███╗ ██╗
██╔══██╗██╔══██╗██║ ██║██╔════╝████╗ ██║
██████╔╝███████║██║ ██║█████╗ ██╔██╗ ██║
██╔══██╗██╔══██║╚██╗ ██╔╝██╔══╝ ██║╚██╗██║
██║ ██║██║ ██║ ╚████╔╝ ███████╗██║ ╚████║
╚═╝ ╚═╝╚═╝ ╚═╝ ╚═══╝ ╚══════╝╚═╝ ╚═══╝

## Requirements

- Python 3.8 or higher
- pip (Python package manager)

## Installation

### 1. Clone or download the repository

```bash
git clone https://github.com/WareIG/hotmail-tiktok-checker.git
cd hotmail-tiktok-checker
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Verify Python version
```bash
python --version
# Should output Python 3.8 or higher
```

## Usage

### Basic usage
```bash
python "Hotmail Tiktok Checker.py"
```

### Input File Format
```text
user1@hotmail.com:password123
user2@outlook.com:MyPass456
user3@live.com:SecurePass789
```

### Example
```text
┌──────────────────────────────────────────────────────────┐
│ 📂 COMBO FILE                                          │
└──────────────────────────────────────────────────────────┘

Combo File (email:pass): combos.txt
Threads (default 5): 10

✅ Loaded 1000 combos
✅ Threads: 10

Press Enter to start checking...
```

### Output
Results are automatically saved in the RaVen-Hit/TikTok_Hits/ folder, organized by follower count:

```text
RaVen-Hit/TikTok_Hits/
├── 1M+_hits.txt
├── 100k-199k_hits.txt
├── 10k-99k_hits.txt
├── 1k-1.9k_hits.txt
└── username_only.txt
```

### Sample Output
```text
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✅ Hit Found
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📧 Email         : user@hotmail.com
🔑 Password      : password123

🎵 TikTok Information:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
👤 Username      : @username
📛 Name          : User Name
👥 Followers     : 150K (150,000)
➕ Following     : 2.5K (2,500)
📹 Videos        : 45
❤️  Likes         : 1.2M (1,200,000)
✅ Verified      : Yes
🔒 Private       : No
🌍 Country       : US 🇺🇸

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
💎 Captured by: @P_N_M
🔗 Channel: https://t.me/dev_raven
⏰ Date: 2026-08-12 14:30:45
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

### Live Display
The tool features a real-time dashboard showing:
- ⚡ Current status
- ✓ Hits found
- ✗ Bad accounts
- 🔒 Secured (2FA) accounts
- ⟳ Retries
- 🎵 TikTok accounts found
- Progress bar
- Speed (CPM)
- Followers ranges
- Linked services
- Current email being checked

### Telegram Integration
The tool sends hits to Telegram channel @dev_raven. To use this feature:

#### 1. Set your Telegram Bot Token in the script
#### 2. Set your Telegram Chat ID

```python
TELEGRAM_BOT_TOKEN = "YOUR_BOT_TOKEN"
TELEGRAM_CHAT_ID = "YOUR_CHAT_ID"
```

## Troubleshooting

### SSL Certificate Errors
```bash
pip install --upgrade certifi
```

### Rate Limiting
Reduce threads to avoid IP blocking:

```bash
# When prompted, enter a lower number
Threads (default 5): 2
```

### No Results Found
- Ensure emails are valid Microsoft accounts
- Check that passwords are correct
- Try increasing threads for faster processing

## Disclaimer
This tool is for educational and security research purposes only. Users are responsible for complying with applicable laws and terms of service.

## Credits
- Creator: @P_N_M
- Channel: @dev_raven
- Version: 1.0.0

## License
MIT License - see LICENSE file for details.
