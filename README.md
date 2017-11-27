# Hardcore ESLint Shareable Config for functional programming

[![Travis CI build status](https://img.shields.io/travis/EvgenyOrekhov/eslint-config-hardcore-fp/master.svg?style=flat-square)](https://travis-ci.org/EvgenyOrekhov/eslint-config-hardcore-fp)

## About

[Shareable Configs](http://eslint.org/docs/developer-guide/shareable-configs)
are designed to work with the `extends` feature of `.eslintrc` files.

This config extends the
[hardcore](https://github.com/EvgenyOrekhov/eslint-config-hardcore)
config and adds rules from
[eslint-plugin-fp](https://github.com/jfmengels/eslint-plugin-fp).

This config is designed to be compatible with Douglas Crockford's
[JSLint](http://jslint.com/).

| Rules                                                                      | Total | Enabled |
| -------------------------------------------------------------------------- | ----: | ------: |
| [ESLint](http://eslint.org/docs/rules/)                                    | 249   | **226** |
| [eslint-plugin-promise](https://github.com/xjamundx/eslint-plugin-promise) | 12    | **9**   |
| [eslint-plugin-fp](https://github.com/jfmengels/eslint-plugin-fp)          | 17    | **15**  |
| **Total**                                                                  | 278   | **250** |

## Usage

First run this:

```bash
npm install eslint-config-hardcore-fp --save-dev
```

Then, add `"extends": "hardcore-fp"` to your .eslintrc file and specify your
[environments](http://eslint.org/docs/user-guide/configuring#specifying-environments):

```json
{
    "extends": "hardcore-fp",
    "env": {
        "node": true,
        "browser": true
    }
}
```

*Note: We omitted the `eslint-config-` prefix since it is automatically assumed
by ESLint.*

You can override settings from the shareable config by adding them directly into
your `.eslintrc` file:

```json
{
    "extends": "hardcore-fp",
    "env": {
        "node": true,
        "browser": true
    },
    "rules": {
        "no-console": "off"
    }
}
```

## License

[MIT](LICENSE)
