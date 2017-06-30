# Airbnb+ JavaScript Standard Style

ESLint on steroids (extends "airbnb" + "standard" configs). Global installation!

It uses original Airbnb Style config extended with JavaScript Standard Style config (with semicolons).

See [airbnb/javascript] and [standardjs] for more information.

[Compare] configs.

[airbnb/javascript]: https://github.com/airbnb/javascript
[standardjs]: https://standardjs.com/
[Compare]: https://npmcompare.com/compare/eslint-config-airbnb,standard

## Installation

Install it globally:

```bash
npm install --global eslint-config-airbnb-standard
```

You can now run feature packed `eslint` from any directory:

```bash
eslint -v
```

Create `.eslintrc` file in your project. Setup your IDE / Editor. Be smart!

ES6, ES7, React, JSX, async/await - all new features supported by default 👍

### WebStorm

File | Settings | Languages and Frameworks | JavaScript | Code Quality Tools | ESLint

![ESLint settings](http://i.imgur.com/ZznYeJU.png)

### Sublime Text 3

1. Install this package globally

2. Go to: *Preferences -> Package Control -> install package*

3. Install [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)

4. Install [SublimeLinter-contrib-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)

5. Run:
    ```bash
    npm bin -g
    ```
    ... and copy the path
6. Go to: *Tools -> SublimeLinter -> Open User Settings*

   Paste the path to NodeJS installation folder inside "paths" for your OS, for example:
    ```json
    "paths": {
        "linux": [
            "~/.nvm/versions/node/v8.1.2/bin"
        ],
        "osx": [],
        "windows": ["%AppData%\\npm"]
    },
    ```
7. Create `.eslintrc` file inside your working project:
    ```json
    {
      "extends": ["airbnb-standard"]
    }
    ```

8. Go to *Tools -> SublimeLinter -> Lint this view*

9. You can switch to squiggly underline mark style from *Tools*.

10. Restart Sublime Text. Have fun!

![Example](http://i.imgur.com/3nzwkdK.png?1)

### Custom Config

You can turn off semicolons in `.eslintrc` (*semi -> "never"*) for your project:

```json
{
  "extends": ["airbnb-standard"],
  "rules": {
    "semi": ["error", "never"]
  }
}
```

### I want that Sublime Text

You can setup full featured nice black Sublime Text 3 from this repo: [sublime-text-3-settings](https://github.com/doasync/sublime-text-3-settings)
