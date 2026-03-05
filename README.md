\# OpenRouter Terminal Chat



Terminal-based chat interface untuk OpenRouter API. Chat dengan AI langsung dari command line tanpa perlu frontend!



\## Features



\- Single query mode - kirim satu pertanyaan langsung

\- Interactive mode - percakapan berkelanjutan

\- Conversation history

\- Clean terminal interface

\- Secure API key management via environment variables



\## Installation



\### 1. Clone repository

```bash

git clone https://github.com/felixgf24gideon-sudo/openrouter-terminal-chat.git

cd openrouter-terminal-chat

```



\### 2. Install dependencies

```bash

pip install -r requirements.txt

```



\### 3. Setup API Key

Dapatkan API key dari \[OpenRouter](https://openrouter.ai/keys)



\*\*Windows PowerShell:\*\*

```powershell

$env:OPENROUTER\_API\_KEY="sk-or-v1-your-api-key-here"

```



\*\*Linux/Mac:\*\*

```bash

export OPENROUTER\_API\_KEY="sk-or-v1-your-api-key-here"

```



Atau buat file `.env`:

```bash

cp .env.example .env

\# Edit .env dan isi API key Anda

```



\## Usage



\### Single Query Mode

```bash

python chat.py "halo"

python chat.py "jelaskan quantum computing"

```



\### Interactive Mode

```bash

python chat-interactive.py

```



Commands dalam interactive mode:

\- `exit` atau `quit` - keluar

\- `clear` - reset percakapan

\- `history` - lihat riwayat chat



\### PowerShell Alias (Windows)

Tambahkan ke PowerShell profile (`$PROFILE`):

```powershell

function chat {

&nbsp;   python C:\\path\\to\\chat.py $args

}



function chati {

&nbsp;   python C:\\path\\to\\chat-interactive.py

}

```



Reload profile:

```powershell

. $PROFILE

```



Sekarang bisa langsung:

```powershell

chat "halo"

chati  # interactive mode

```



\## Requirements



\- Python 3.7+

\- requests library

\- OpenRouter API key



\## 📄 License



MIT License - lihat \[LICENSE](LICENSE) file



\##  Contributing



Pull requests welcome! Untuk perubahan besar, silakan buka issue dulu.



\## Author



\*\*felixgf24gideon-sudo\*\*



\## Acknowledgments



\- \[OpenRouter](https://openrouter.ai/) - AI API Gateway

\- Terinspirasi dari kebutuhan chat terminal yang simple

