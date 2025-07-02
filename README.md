<img src="https://github.com/user-attachments/assets/43306087-42cf-48fb-b118-0c416d65835a" alt="kcme" width="300"/>    

# kcme
### Simplified Kerberos ccache management. No more need to remember realms.

# Description
This was developed to solve the issue of managing the ccache file while negotiating with Kerberos. The tool 𝗸𝗰𝗺𝗲 essentially takes simple parameters, uses the provided IP address and does a lookup of domains in /etc/hosts. The tool will attempt each domain so the user doesn't need to remember the correct realm name and also all domain are translated to UPPERCASE for kinit generation.

# Install
```
sudo wget https://github.com/DaddyBigFish/kcme/raw/refs/heads/main/kcme -O /usr/local/bin/kcme
sudo chmod +x /usr/local/bin/kcme
echo 'export KRB5CCNAME=/tmp/krb5cc_1000' >> ~/.zshrc
echo 'export KRB5CCNAME=/tmp/krb5cc_1000' >> ~/.bashrc
source ~/.zshrc ~/.bashrc
```
# Usage
```
kcme 'kaorz:Roper4155'@10.10.10.240
Password for kaorz@LICORDEBELLOTA.HTB:
Ticket cache: FILE:/tmp/krb5cc_1000
Default principal: kaorz@LICORDEBELLOTA.HTB

Valid starting       Expires              Service principal
07/02/2025 12:31:08  07/02/2025 22:31:08  krbtgt/LICORDEBELLOTA.HTB@LICORDEBELLOTA.HTB
        renew until 07/03/2025 12:31:08
```
