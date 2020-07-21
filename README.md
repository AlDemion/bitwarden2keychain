# bitwarden2keychain
Shell script to add passwords from Bitwarden to MacOS Keychain

## Installation
Just download this script and make it executable. Exemple you can find below.

```bash
curl -L -o bitwarden2keychain https://github.com/aldemion/bitwarden2keychain/releases/download/1.0/bitwarden2keychain
chmod +x bitwarden2keychain
```

If you want to use this script regulary place it in the directory that exists in your PATH, like below.

```bash
sudo mv bitwarden2keychain /usr/local/bin
```

## Help
To display usage message call script with "-h" option.

```bash
usage: ./bitwarden2keychain [-l <Bitwarden login>]
  -l <Bitwarden login>
  -m <Bitwarden 2FA method>
  -u <Bitwarden server URL> If not provided - default url will be used.
  -h Print this message and exit.

     This application tries to login to Bitwarden server, get stored passwords
     and import them to MacOs Keychain as "internet-password".
     You can also specify your own Bitwarden server URL.
     Also, Bitwarden cli tool required for this script.
     You can find bitwarden cli installation instructions here:
     https://bitwarden.com/help/article/cli/#download--install
```