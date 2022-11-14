# Bootstrap Steps

Wait for Ubuntu to boot into the login screen.

Log in as the vagrant user.

Click or press enter to accept defaults for anything it asks, such as:

* LivePatch registration
* System reporting
* Location services
* Suggested software

Wait for the upgrade prompt to appear and choose "Don't upgrade".

Open a Terminal.

Add a Spanish keyboard layout. ([Source](https://askubuntu.com/a/1033461/143624))

```bash
gsettings set org.gnome.desktop.input-sources sources \
"[('xkb', 'es'), ('xkb', 'us')]"
```

Set Spanish as the current layout. The "0" indexes refers to the array declared in the previous command. ([Source](https://askubuntu.com/a/1176729/143624))

```bash
gdbus call \
--session \
--dest org.gnome.Shell \
--object-path /org/gnome/Shell \
--method org.gnome.Shell.Eval "imports.ui.status.keyboard.getInputSourceManager().inputSources[0].activate()"
```

Install [chezmoi](https://www.chezmoi.io/) with the following commands.

```bash
PATH="$PATH:$HOME/.local/bin"
sh -c "$(curl -fsLS get.chezmoi.io)" -- -b $HOME/.local/bin
```

Init the home folder and apply my latest chezmoi settings.

```bash
chezmoi init --apply "https://github.com/iainelder/chezmoi"
```

Generate a temporary SSH key.

```bash
ssh-keygen
```

Copy the key to your Github settings.

Perform chezmoi commands to continue building the environment from inside the virtual machine.

## Restore Thunderbird profile

See "Borg: Try to restore to a different computer" for inspiration.

```bash
cd "$(mktemp --dir)"

borg extract --list "::full_system_2022-11_12_15:33" home/isme/.thunderbird
```

## Every day use

Start the 1Password GUI application.

Log into the 1Password GUI.

Log into the 1Password CLI.

```bash
op signin my.1password.com iainelder@hotmail.co.uk
```

Start Firefox.

Log into your Firefox account to sync the browser data and configuration.
