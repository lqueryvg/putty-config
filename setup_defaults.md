# Setup Session Defaults

These steps configure defaults for the `Default Settings` Putty session.
This session can be used as the basis for creating new sessions.

## Quick Setup

- edit [`Default_Settings.reg`](Default_Settings.reg), change the first three lines of settings to reflect the correct:
  - log file location
  - typical user name (that you will log in as)
  - private key file (despite the registry name "PublicKeyFile", this **is** the private key not the public)
    - if you don't have a public / private key pair, create one with [PuTTYgen](https://www.ssh.com/ssh/putty/windows/puttygen) (which is supplied with Putty)
- Import  [`Default_Settings.reg`](Default_Settings.reg) into the registry (double-click in explorer)

Tips:

- you can manually edit [`Default_Settings.reg`](Default_Settings.reg) and re-import it later
- delete lines completely if there are certain settings which you don't want to overwrite
- change the session name to create multiple sets of defaults or to import sets of settings into existing sessions

## Manual Setup

Follow these steps if you prefer the pain and glory of doing this by hand.

### Steps

1. [Open New Session Dialog](#open-new-session-dialog)
1. [Load Default Settings](#load-default-settings)
1. [Logging](#logging) (smart logfile name)
1. [Window](#window) (size & scrollback)
1. [Appearance](#appearance) (font and cursor)
1. [Selection](#selection) (mouse selection style)
1. [Colours](#colours)
1. [Data](#data) (terminal type and user name)
1. [Auth](#auth) (ssh private key)
1. [X11 Forwarding](#x11-forwarding)
1. [Save (**IMPORTANT**)](#save-defaults)

### Open New Session Dialog

![Open New Session Dialog](pictures/01_NewSession.PNG)

### Load Default Settings

![Load Default Settings](pictures/02_LoadDefaultSettings.png)

### Logging

- Click `Browse` to set directory.
- Use cookies to set a unique filename for every session, e.g.: `C:\Users\John\Documents\putty_logs\&Y&M&D_&T_&H.log`

![Logging](pictures/defaults/Logging.png)

### Window

![Window](pictures/defaults/Window.png)

### Appearance

![Appearance](pictures/defaults/Appearance.png)

### Selection

![Selection](pictures/defaults/Selection.png)

### Colours

If you want to manually tweak the colours, do it here...
![Colours](pictures/defaults/Colours.png)

### Data

![Data](pictures/defaults/Data.png)

## SSH Compression

Enabling compression improves performance with X11 forwarding over Virtualbox NAT interfaces.

![Data](pictures/defaults/SSH.png)

### Auth

![Auth](pictures/defaults/Auth.png)

### X11 Forwarding

![X11](pictures/defaults/X11.png)

### Save Defaults

![Save Defaults](pictures/defaults/SaveDefaults.png)
