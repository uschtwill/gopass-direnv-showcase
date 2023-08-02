# gopass-direnv-showcase

1. Install `direnv`: https://direnv.net/#basic-installation
2. Create a `gpg` key: https://github.com/gopasspw/gopass/blob/master/docs/setup.md#set-up-a-gpg-key-pair
3. Send me the public part of your `gpg` key, so I can add you to the users of our password store. Example command: `gpg --output alice.gpg --export alice@cyb.org`
4. Install `gopass`: https://github.com/gopasspw/gopass/blob/master/docs/setup.md#macos-1
5. Clone our password store: `gopass clone git@>>OUR_PASSWORD_STORE<<`
6. Clone this showcase repository: `git clone git@github.com:uschtwill/gopass-direnv-showcase.git`
7. `cd` into the directory and run `direnv allow` to allow `direnv` to work here.
8. The secrets should be loaded now, if not `cd` out of and back into the directory.
9. `direnv` should now have loaded the secrets for you, maybe prompting you to insert your gpg key passphrase (if it's not within the cooldown).
10. Run `node index.js`, the rest is history.
