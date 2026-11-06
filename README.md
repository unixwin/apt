# niubash APT archive

Signed Debian/Ubuntu packages for [niubash](https://github.com/unixwin/niubash).

```bash
curl -fsSL https://unixwin.github.io/apt/KEY.gpg | sudo gpg --dearmor -o /usr/share/keyrings/niubash-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/niubash-archive-keyring.gpg] https://unixwin.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/niubash.list
sudo apt update && sudo apt install niubash
```

Suites: `stable` (amd64, arm64). glibc floor 2.35: Ubuntu 22.04+, Debian 12+.
Populated automatically by niubash's apt-repo workflow (reprepro, GPG-signed InRelease).
