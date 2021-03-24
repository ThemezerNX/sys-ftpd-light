# sys-ftpd

This is a nintendo-switch sysmodule which runs an ftpd-server in the background. This fork adds a custom `REB` FTP command that reboots the console.

Hotkeys:  
You can toggle the state of the server using the (+) + (-) + (X) button combination.

---

Config Example (Located on your sd in `sdmc:/config/sys-ftpd/config.ini`):

```
[User]
user:=nxthemer

# user:= -> Login username

[Password]
password:=nxthemer

# password:= -> Login password

[Port]
port:=5000

# port:=5000 -> opens the server on port 5000 (using the console's IP address).

[Anonymous]
anonymous:=1

# anonymous:=1 -> Allows logging into the ftpd server without username or password.
# anonymous:=0 -> Only allows logging into the ftpd server with the correct username and password. user and password (in fields above) must be set.

[Pause]
disabled:=0
keycombo:=PLUS+MINUS+X

# disabled:=1 -> Disables allowing sys-ftpd to be paused by pressing the key combination.
# disabled:=0 -> Allows sys-ftpd to be paused by pressing the key combination.
# keycombo:=  -> The key combination used to pause sys-ftpd. Each key is separated by either a plus '+' or a space ' '. Up to 8 keys are allowed.
# The list of valid keys is as follows:
# A, B, X, Y, LS, RS, L, R, ZL, ZR, PLUS, MINUS, DLEFT, DUP, DRIGHT, DDOWN

[LED]
led:=1

# led:=1 -> LED flashes on connect (default)
# led:=0 -> LED does not flash on connect
```
