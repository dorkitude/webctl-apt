# webctl apt repository

Signed Debian packages for [webctl](https://github.com/dorkitude/webctl), published by its release workflow and served over GitHub Pages.

```bash
curl -fsSL https://dorkitude.github.io/webctl-apt/key.gpg | sudo gpg --dearmor -o /usr/share/keyrings/webctl.gpg
echo "deb [signed-by=/usr/share/keyrings/webctl.gpg] https://dorkitude.github.io/webctl-apt stable main" | sudo tee /etc/apt/sources.list.d/webctl.list
sudo apt update && sudo apt install webctl
```
