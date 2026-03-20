<h1 align="center">MaxPhisher</h1>

<p align="center">
  Educational Cybersecurity Tool for Demonstrating Phishing Techniques
</p>

---

## 📄 Description

MaxPhisher is a **Python-based educational tool** designed to demonstrate phishing techniques, social engineering concepts, and user awareness in cybersecurity.

It is intended strictly for:
- 🎓 Learning purposes  
- 🔐 Ethical penetration testing (with permission)  
- 🧠 Security awareness training  

---

## ⚠️ Disclaimer

> 🚨 This project is for **educational purposes only**.  
> Unauthorized use against systems or individuals without explicit permission is illegal and unethical.  
> The author is not responsible for misuse.

---

## ✨ Features

- 🌐 Multi-platform support (Linux-based systems)
- 🎭 Multiple simulated templates (100+)
- 🔗 URL masking & redirection techniques (for demonstration)
- 📡 Tunneling support (Cloudflared, LocalXpose, etc.)
- 📊 Demonstrates data capture concepts in controlled environments
- 🛠️ Easy-to-use interface for learning purposes

---

## 💻 Supported Platforms

| OS        | Support Level |
|----------|--------------|
| Linux     | ✅ Excellent |
| Android   | ✅ Excellent |
| macOS     | ⚠️ Alpha (Docker Recommended) |
| iOS       | ⚠️ Alpha (Docker Recommended) |
| Windows   | ❌ Unsupported (Use VM/Docker) |

---

## 🛠️ Installation

### 🔧 Install Dependencies

**Debian (Ubuntu, Kali, Parrot):**
```bash
sudo apt install git python3 python3-pip php openssh-client -y
 - For Debian (Ubuntu, Kali-Linux, Parrot)
    - ```sudo apt install git python3 python3-pip php openssh-client -y```
 - For Arch (Manjaro)
    - ```sudo pacman -S git python3 python-pip php openssh --noconfirm```
 - For Redhat(Fedora)
    - ```sudo dnf install git python3 php openssh -y```
 - For Termux
    - ```pkg install git python3 python-pip php openssh -y```

##### Clone this repository

 - ```git clone https://github.com/soksereyvathna-uk/CredentialPhisher.git```

##### Enter the directory
 - ```cd MaxPhisher```

##### Install all modules
 - ```pip3 install -r files/requirements.txt --break-system-packages```

##### Run the tool
 - ```python3 maxphisher.py```

#### Or, directly run
```
wget https://raw.githubusercontent.com/soksereyvathna-uk/MaxPhisher/main/maxphisher.py && python3 maxphisher.py

```

### Pip
 - `pip3 install maxphisher` [For Termux]
 - `sudo pip3 install maxphisher --break-system-packages` [For Linux]
 - `maxphisher`

### Docker

 - `sudo docker pull soksereyvathna-uk/maxphisher`
 - `sudo docker run --rm -it soksereyvathna-uk/maxphisher`
 - `sudo docker cp $(sudo docker ps | grep maxphisher | awk '{print $1}'):/root/Media media` 


### Support

OS         | Support Level
-----------|--------------
Linux      | Excellent
Android    | Excellent
iPhone     | Alpha (Recommended docker)
MacOS      | Alpha (Recommended docker)
Windows    | Unsupported (Use docker/virtual-box/vmware)
BSD        | Never tested

#### Options

```
usage: maxphisher.py [-h] [-p PORT] [-t TYPE] [-o OPTION]
                     [-T TUNNELER] [-r REGION] [-S SUBDOMAIN]
                     [-d DIRECTORY] [-f FEST] [-i YTID] [-u URL]
                     [-s DURATION] [-m MODE] [-e TROUBLESHOOT]
                     [--nokey] [--noupdate]

options:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  MaxPhisher's server port [Default : 8080]
  -t TYPE, --type TYPE  MaxPhisher's phishing type index [Default :
                        null]
  -o OPTION, --option OPTION
                        MaxPhisher's template index [ Default : null ]
  -T TUNNELER, --tunneler TUNNELER
                        Tunneler to be chosen while url shortening
                        [Default : Cloudflared]
  -r REGION, --region REGION
                        Region for loclx [Default: auto]
  -S SUBDOMAIN, --subdomain SUBDOMAIN
                        Subdomain for loclx [Pro Account]
                        (Default: null)
  -d DIRECTORY, --directory DIRECTORY
                        Directory where media files will be saved
                        [Default : /sdcard/Media]
  -f FEST, --fest FEST  Festival name for fest template [Default:
                        Birthday]
  -i YTID, --ytid YTID  Youtube video ID for yttv template [Default :
                        6hHmkInZkMQ (NASA Video)]
  -u URL, --url URL     Redirection url for ip-tracking or login
                        phishing [Default : null]
  -s DURATION, --duration DURATION
                        Media duration while capturing [Default :
                        5000(ms)]
  -m MODE, --mode MODE  Mode of MaxPhisher [Default: normal]
  -e TROUBLESHOOT, --troubleshoot TROUBLESHOOT
                        Troubleshoot a tunneler [Default: null]
  --nokey               Use localtunnel without ssh key [Default:
                        False]
  --noupdate            Skip update checking [Default : False]
```

### Features:

 - Multi platform (Supports most linux)
 - 100+ templates
 - Concurrent 4 tunneling (Cloudflared and LocalXpose, LocalHostRun, Serveo)
 - OTP Support
 - Credentials mailing
 - Easy to use
 - Possible error diagnoser
 - Built-in masking of URL
 - Custom masking of URL
 - URL Shadowing
 - Portable file (Can be run from any directory)
 - Get IP Address and many other details along with login credentials


### Requirements

 - `Python(3)`
   - `requests`
   - `rich`
   - `beautifulsoup4`
 - `PHP`
 - `SSH`
 - 900MB storage
 
If not found, php, ssh and python modoules will be installed on first run

#### Tested on

 - `Termux`
 - `Ubuntu`
 - `Kali-Linux`
 - `Arch`
 - `Fedora`
 - `Manjaro`

## Usage

1. Run the script
2. Choose a Website
3. Wait sometimes for setting up all
4. Send the generated link to victim
5. Wait for victim login. As soon as he/she logs in, credentials will be captured


 
## Solution of common issues
 - Some secured browsers like Firefox can warn for '@' prefixed links. You should use pure links or custom link to avoid it.
 - Termux from play store in not supported. Download termux from fdroid or github
 - VPN or proxy prevents tunneling and even proper internet access. Turn them off you have issues.
 - Some android requires hotspot to start Cloudflared and Loclx. If you face 'tunneling failed' in android, most probably your hotspot is turned off. Turn it on and keep it on untill you close MaxPhisher.


## [!] Disclaimer
***This tool is developed for educational purposes. Here it demonstrates how phishing works. If anybody wants to gain unauthorized access to someones social media, he/she may try out this at his/her own risk. You have your own responsibilities and you are liable to any damage or violation of laws by this tool. The author is not responsible for any misuse of MaxPhisher!***



## Credits:
[PyPhisher](https://github.com/KasRoudra/PyPhisher)
[CamHacker](https://github.com/KasRoudra/CamHacker)
[VidPhisher](https://github.com/KasRoudra/VidPhisher)
[IP-Tracker](https://github.com/KasRoudra/IP-Tracker)
[Storm-Breaker](https://github.com/ultrasecurity/Storm-Breaker)
[Seeker](https://github.com/thewhiteh4t/seeker)



