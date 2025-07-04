<img src="https://github.com/user-attachments/assets/43306087-42cf-48fb-b118-0c416d65835a" alt="kcme" width="300"/>    

# kcme
### Simplified Kerberos ccache management.

# Description
This was developed to solve the issue of managing ccache files while negotiating with Kerberos. The tool 𝗸𝗰𝗺𝗲 essentially provides a simple management user interface in python. It reads available .ccache files in the current directory and allows the user to select the user they wish to use for Kerberos negotiation. Once a user is selected, it loads the file into /tmp/krb5cc_1000.

# Requirements
```
sudo apt install krb5-user
echo 'export KRB5CCNAME=/tmp/krb5cc_1000' >> ~/.zshrc
echo 'export KRB5CCNAME=/tmp/krb5cc_1000' >> ~/.bashrc
source ~/.zshrc ~/.bashrc
```
# Install
```
sudo wget https://github.com/DaddyBigFish/kcme/raw/refs/heads/main/kcme -O /usr/local/bin/kcme
sudo chmod +x /usr/local/bin/kcme
```
# Usage
```
kcme
┌──────────────────────────────────────────┐
│   Kerberos Negotiation Management Menu   │
│             by DaddyBigFish              │
└──────────────────────────────────────────┘
=> 1. kaorz
=> 2. gibdeon
=> 3. lothbrok
=> 4. 0xvic
=> 5. administrator
=> 6. backupadmin
```
