---
layout: post
title: Verified commits
---

<div class="max-300 margin-auto-h padding-b-40">
  <img class="box-shadow" src="http://i.imgur.com/NulTUck.png" alt="verified commit" />
</div>

- Install gpg1:
  - `brew install gpg1`

- Set the encoding as utf-8:
  - `vim ~/.gnupg/gpg.conf` then uncomment `charset utf-8`

- Check if you already have GPG keys installed
  - `gpg --list-secret-keys --keyid-format LONG`
- If not, generate a new one:
  - `gpg --gen-key`
- Get the public key:
  - `gpg --armor --export ABCDEF`
  - Paste that on https://github.com/settings/keys
- Configure git to always sign commits with this key:
  - `git config --global gpg.program gpg1`
  - `git config --global commit.gpgsign true`
  - `git config --global user.signingkey ABCDEF`
- Get gpgtools to store passphrase in MacOS:
  - `brew cask install gpgtools` (requires sudo access)
  - Open "GPG Keychain", select key, "change passphrase", "store in keychain"
- **Commit like usual**:
  - `git commit ...`
  - `git merge ...`
  - `git pull ...`

