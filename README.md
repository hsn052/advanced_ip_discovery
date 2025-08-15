🛠️ Installation
Prerequisites
bash# Python 3.6+ tələb olunur
python3 --version

# Tələb olunan paketlər
pip install requests dnspython

# WHOIS tool (Linux/macOS)
# Ubuntu/Debian:
sudo apt-get install whois

# CentOS/RHEL:  
sudo yum install whois

# macOS:
brew install whois
Download
bashgit clone https://github.com/yourusername/advanced-ip-discovery.git
cd advanced-ip-discovery
chmod +x advanced_ip_discovery.py
🚀 Usage
Basic Usage (Domain only)
bashpython3 advanced_ip_discovery.py
Sonra domain daxil edin: example.com
Advanced Usage (Domain + Subdomain file)
bashpython3 advanced_ip_discovery.py

Domain: example.com
Subdomain file: subdomains.txt

📄 Subdomain File Format
Tool aşağıdakı formatları dəstəkləyir:
Full Domain Format (Recommended)
www.example.com
mail.example.com
api.example.com
admin.panel.example.com
Simple Subdomain Format
www
mail
ftp
admin
api
Mixed Format
www.example.com
mail
api.internal.example.com
ftp
 Output Example
ÜMUMİ STATİSTİKA:
   • Aktiv domain-lər: 15
   • Unikal IP-lər: 8
   • Tarixi IP-lər: 3
   • WHOIS məlumatları: 5

DOMAIN-LƏR VƏ IP-LƏR:
   [www.example.com]
     A Records: 93.184.216.34
     MX Records: 10 mail.example.com

 BÜTÜN TAPILAN IP-LƏR:
     1. 93.184.216.34 (Example Corp, US)
     2. 192.168.1.100 (Local Hosting, AZ)
     3. 52.101.73.1 (Microsoft, US)

IP ARALIQLARI:
     • 93.184.216.x: ['93.184.216.34', '93.184.216.35']
Output Files
Tool nəticələri JSON formatında saxlayır:

domain_ip_discovery.json - Bütün məlumatları strukturlaşdırılmış formatda
