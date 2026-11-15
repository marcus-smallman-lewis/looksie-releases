# Looksie

Have a proper looksie at big pull requests. Looksie is a desktop app for Windows and Mac that walks you through a big
pull request one decision at a time, then posts your review.

This repository holds the downloads and the website. **[Download the latest version](https://github.com/marcus-smallman-lewis/looksie-releases/releases/latest)**

## Installing

Preview builds are not signed yet, so the first time you open Looksie your computer will ask if you are sure.

**Windows:** run `Looksie-windows-setup.exe`. If SmartScreen says it protected your PC, click **More info**, then **Run anyway**.

**Mac:** use `Looksie-mac-apple-silicon.dmg` for a Mac with an Apple chip (M1 and later), or `Looksie-mac-intel.dmg` for an
older Intel Mac (Apple menu → About This Mac says which). Open the .dmg and drag Looksie into Applications. Open it once,
press Done at the warning, then go to **System Settings → Privacy & Security** and click **Open Anyway**.

If the Mac says the app is damaged, run this in Terminal, then open it again:

    xattr -dr com.apple.quarantine /Applications/Looksie.app

After that, Looksie keeps itself up to date: it checks once a day and installs a new version when you say.
