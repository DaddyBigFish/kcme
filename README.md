# kcme
### Simplified Kerberos ccache management. No more need to remember realms.

# Description
This was developed to solve the issue of managing the ccache file while negotiating with Kerberos. The tool 𝗸𝗰𝗺𝗲 essentially takes simple parameters, and uses the provided IP address in order to lookup the domains in /etc/hosts. The tool will attempt each domain so the user doesn't need to remember the correct realm name and also all domain are translated to UPPERCASE for kinit generation.

# Install
```
wget https://github.com/DaddyBigFish/skewme/raw/refs/heads/main/skewme -O /usr/local/bin/skewme
sudo chmod +x /usr/local/bin/kcme
```
# Usage
```
sudo kcme 'username:password'@xx.xx.xx.xx
```
