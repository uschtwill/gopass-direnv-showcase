# gopass-direnv-showcase

1. Install `direnv`: https://direnv.net/#basic-installation
2. Make sure it's hooked into your shell: https://direnv.net/docs/hook.html
3. Create a `gpg` key: https://github.com/gopasspw/gopass/blob/master/docs/setup.md#set-up-a-gpg-key-pair
4. Send me the public part of your `gpg` key, so I can add you to the users of our password store. Example command: `gpg --output alice.gpg --export alice@cyb.org`
5. Install `gopass`: https://github.com/gopasspw/gopass/blob/master/docs/setup.md#macos-1
6. Clone our password store: `gopass clone git@>>OUR_PASSWORD_STORE<< seven-one`
7. Clone this showcase repository: `git clone git@github.com:uschtwill/gopass-direnv-showcase.git`
8. `cd` into the directory and run `direnv allow` to allow `direnv` to work here.
9. The secrets should be loaded now, if not `cd` out of and back into the directory.
10. `direnv` should now have loaded the secrets for you, maybe prompting you to insert your gpg key passphrase (if it's not within the cooldown).
11. Run `node index.js`, the rest is history.
