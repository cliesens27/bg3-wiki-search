<img src="src/icons/icon_152.png"/>

# Baldur's Gate 3 Wiki search

This is a fork of the [Path of Exile Wiki Search Extension](https://github.com/Project-Path-of-Exile-Wiki/poe-wiki-search); credits go to [pm5k](https://github.com/pm5k) and the PoE community.

This is a browser extension designed to be used in Firefox, Google Chrome, and chromium-based browsers (such as MS Edge) by players of the popular CRPG - [Baldur's Gate 3](https://baldursgate3.game/). This extension provides a single, simple feature : upon pressing `Alt+A` (defined in the `"commands"` section in `src/manifest.json`), a small popup opens allowing the user to search for information about the game using the [community wiki](www.bg3.wiki). Unlike the [other extension](https://github.com/Project-Path-of-Exile-Wiki/poe-wiki-search) referenced above, this one performs no redirection of any kind, and simply allows you to search the official community wiki at the press of a button. That's it!

# Dev quickstart

## Recommended setup

- [pnpm](https://pnpm.io/) (although you can use npm or yarn)
- [web-ext](https://github.com/mozilla/web-ext)

## Installation steps

- `npm i -g pnpm` <-- the last time you'll ever use NPM if you decided to switch to PNPM,
- `git clone https://github.com/cliesens27/bg3-wiki-search`
- `pnpm i -g web-ext`
- `cd /path/to/bg3-wiki-search`,
- `pnpm install`
- `pnpm run start`

Now every time you make changes to the code, you'll see them live on Firefox. Unless you do something browser-specific in the code, your
extension should just work almost everywhere!

## Build

To build your extension for publishing, simply run `pnpm run build`. The packaged zip file will be output to `build/`.

# FAQ

## Is this extension safe?

Yes, it is. We do not enforce its use, we provide it as a means to simplify your life for searching for Baldur's Gate 3 related information using the official wiki directly. The code that does this sits in `src/ui/ui.js`.

Each file has a laymanised comment stack to walk even non-technical users through what it does and why. Don't be shy and read through!

## Do you collect any data?

Absolutely not. This extension does not need anything from you to work. No information is read, asked for or needed. At all.

## I want to contribute, how do I do this?

Just fork the repo, add your changes and submit a PR.