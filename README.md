# public_json_bin

A tidy bucket of JSON that my apps and CLIs fetch at runtime over `raw.githubusercontent.com`. Editing a file here updates every client instantly — no app release, no server, free hosting.

Think of it as the organised successor to [SomeHowTosAndTexts](https://github.com/p32929/SomeHowTosAndTexts).

## Layout

```
_commons/    shared payloads (e.g. a default updater.json)
android/     data for Android apps (motivational updates, …)
clis/        data for CLI tools (siin.json = the app list for siin)
web/         data for web apps (duas.json, send-money links, …)
             web/deprecated/  old versions kept for compatibility
```

## How it's used

A client hardcodes a raw URL and reads it. For example, [siin](https://github.com/p32929/siin) pulls its installable-app list from:

```
https://raw.githubusercontent.com/p32929/public_json_bin/master/clis/siin.json
```

and [duas](https://github.com/p32929/duas) reads `web/duas.json` the same way.

Each file is plain JSON — open it, edit it, commit, and clients pick up the change on their next fetch.

## Contributing

Contributions are warmly welcomed and greatly appreciated! Whether it's a bug fix, new feature, or improvement, your input helps make this project better for everyone.

Before submitting a pull request, please:

1. Create an issue describing the feature or bug fix you'd like to work on
2. Wait for discussion and approval to ensure alignment with project goals
3. Fork the repository and create your feature branch
4. Submit your pull request with a clear description of changes

This approach helps avoid duplicate efforts and ensures smooth collaboration. Thank you for considering contributing!

## Share

Sharing this repository with your friends is just one click away from here

[![facebook](https://user-images.githubusercontent.com/6418354/179013321-ac1d1452-0689-493f-9066-940cf2302b6e.png)](https://www.facebook.com/sharer/sharer.php?u=https://github.com/p32929/public_json_bin/)
[![twitter](https://user-images.githubusercontent.com/6418354/179013351-7d8d6d1c-4ce2-46ab-bef8-4c4765a1b888.png)](https://twitter.com/intent/tweet?url=https://github.com/p32929/public_json_bin/)
[![tumblr](https://user-images.githubusercontent.com/6418354/179013343-3111f55a-3b90-40c7-8487-9777348672b0.png)](https://www.tumblr.com/share?v=3&u=https://github.com/p32929/public_json_bin/)
[![pocket](https://user-images.githubusercontent.com/6418354/179013334-b095c45f-becf-49f4-9ee1-5a731a9b1f85.png)](https://getpocket.com/save?url=https://github.com/p32929/public_json_bin/)
[![pinterest](https://user-images.githubusercontent.com/6418354/179013331-44cd9206-11b1-4b65-becb-5863b61c828f.png)](https://pinterest.com/pin/create/button/?url=https://github.com/p32929/public_json_bin/)
[![reddit](https://user-images.githubusercontent.com/6418354/179013338-7416ae3f-73ba-4522-86e1-1374d7082d22.png)](https://www.reddit.com/submit?url=https://github.com/p32929/public_json_bin/)
[![linkedin](https://user-images.githubusercontent.com/6418354/179013327-ca7b7102-1da8-4b1c-858f-1a6e5f21bd70.png)](https://www.linkedin.com/shareArticle?mini=true&url=https://github.com/p32929/public_json_bin/)
[![whatsapp](https://user-images.githubusercontent.com/6418354/179013353-f477fa0b-3e6f-4138-a357-c9991b23ff88.png)](https://api.whatsapp.com/send?text=https://github.com/p32929/public_json_bin/)
