# "fuck", an ireverent password manager

Derived from the pwd.sh password manager, fuck adds a non-interactive mode with clipboard integration with Macs, and more flexible password store capabilities


# Installation

    git clone https://github.com/jpwarren00/fuck

    from /usr/local/bin

    ln -s {path to fuck}/fuck
    
Requires `gpg`

Install with `brew install gpg` or `sudo apt-get install gnupg` or build and install it from [source](https://www.gnupg.org/download/index.html).

# Use

Run the script interactively with `fuck` or `fuck all`
    
Type `w` to write a password.

Type `r` to read a password or all passwords.

Type `d` to delete a password.

The encrypted file `~/old.list` and script can be safely shared between machines over public channels (Google Drive, Dropbox, etc).

Run the script non-interactively with `fuck {password nickname}` and the script copies the password to your clipboard (Mac only).

Run the script non-interactively with a different password store with `fuck {password nickname} {password store path}` (Mac only).

Run the script interactively with a different password store with `fuck all {password store path}`.

A sample `gpg.conf` configuration file is provided for your consideration.
