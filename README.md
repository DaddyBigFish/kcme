<img src="https://github.com/user-attachments/assets/43306087-42cf-48fb-b118-0c416d65835a" alt="kcme" width="300"/>    

# kcme
### Simplified Kerberos ccache management. No more need to remember realms.

# Description
This was developed to solve the issue of managing the ccache file while negotiating with Kerberos. The tool 𝗸𝗰𝗺𝗲 essentially takes simple parameters, uses the provided IP address and does a lookup of domains in /etc/hosts. The tool will attempt each domain so the user doesn't need to remember the correct realm name and also all domain are translated to UPPERCASE for kinit generation. The extra bonus of 𝗸𝗰𝗺𝗲 is that it works well with tmux and will refresh all tmux panes to receive the new KRB5CCNAME so the user doesn't need to constantly export to each pane.

# Install
```
wget https://github.com/DaddyBigFish/skewme/raw/refs/heads/main/skewme -O /usr/local/bin/skewme
sudo chmod +x /usr/local/bin/kcme
```
# Usage
```
sudo kcme 'username:password'@xx.xx.xx.xx
```
