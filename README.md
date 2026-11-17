# public_json_bin

A small, tidy collection of JSON files that my apps and command line tools read at runtime from `raw.githubusercontent.com`. Change a file here, and every app that reads it gets the new data on its next fetch. There is no app release to ship and no server to run, and the hosting is free.

It is the organised successor to [SomeHowTosAndTexts](https://github.com/p32929/SomeHowTosAndTexts).

## What is inside

```
_commons/    shared files, like a default updater.json
android/     data for Android apps (for example motivate/updates.json)
clis/        data for command line tools (siin.json is the app list for siin)
web/         data for web apps (duas.json, send_money_2_me.json)
             web/deprecated/ keeps old versions for apps that still read them
```

## How apps use it

An app reads a fixed raw link. For example, [siin](https://github.com/p32929/siin) gets its list of apps to install from:

```
https://raw.githubusercontent.com/p32929/public_json_bin/master/clis/siin.json
```

and [Duas](https://github.com/p32929/duas) reads `web/duas.json` the same way.

## Good to know

1. Every file is plain JSON. Open it, edit it, commit it, and the apps pick up the change.
2. GitHub caches raw files for a few minutes, so a change can take a short while to show up.
3. Don't rename or move a file that an app already reads, or that app stops finding it. Copy it to a new name instead, like the files in `web/deprecated/`.

## Contributing

Contributions are very welcome. Please open an issue first to talk about what you'd like to add or change, so we can agree on it before you spend time on a pull request. Thank you!

<p><a href="https://p32929.github.io/share/?repo=public_json_bin"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-share-dark.svg"><img src="https://p32929.github.io/readme/footer-share-light.svg" width="50%" align="top" alt="Share this project with your friends in one click"></picture></a><a href="https://p32929.github.io/support/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-support-dark.svg"><img src="https://p32929.github.io/readme/footer-support-light.svg" width="50%" align="top" alt="If you like my work and want to support me, feel free to support"></picture></a><br><a href="https://openstore.pfay.workers.dev/add"><picture><source media="(prefers-color-scheme: dark)" srcset="https://p32929.github.io/readme/footer-join-dark.svg"><img src="https://p32929.github.io/readme/footer-join-light.svg" width="100%" align="top" alt="Put your own apps on OpenStore: free, your listing lives in your own repo"></picture></a></p>
