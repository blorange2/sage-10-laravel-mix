## Overview

This is a fork of the Sage 10 WordPress starter theme by Roots that uses Laravel Mix and the Bootstrap CSS framework (at current this is version 5).

My reasoning was the fact that Bud.js is a really cool build tool but I didn't want to move everything onto WSL.

## How to include in project

If you want to use this theme in your WordPress project you can either:

1. Clone it inside of your `themes` folder e.g. `git clone https://github.com/blorange2/sage-10-laravel-mix.git your-theme-folder`
2. Require it via Composer like so:

Open your WordPress project's `composer.json` file and add a repository entry for the modified Sage 10 theme. Add the following lines inside the `repositories` section:

```json
"repositories": [
    {
        "type": "vcs",
        "url": "https://github.com/blorange2/sage-10-laravel-mix"
    }
],
```

Then add the package to your list of required packages.

```json
"require": {
    "blorange2/sage-10-laravel-mix": "master"
},
```

## Building

As this theme uses Laravel Mix, in order to build assets you must navigate to your theme folder and run the command `mix` with either Yarn or NPM.

You can see a full listing of the available commands in the `package.json` file.
