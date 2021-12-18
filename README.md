# template-angular-package

[![CI](https://github.com/mrahhal/template-angular-package/actions/workflows/ci.yml/badge.svg)](https://github.com/mrahhal/template-angular-package/actions/workflows/ci.yml)
[![npm](https://img.shields.io/npm/v/template-angular-package.svg)](https://www.npmjs.com/package/template-angular-package)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.txt)

A template for an angular package.

This is for my own use, but feel free to use it if it helps you. The CI workflow uses a shared workflow of mine from another repo, it might change without notice.

## Features

- Angular 13
- [Jest](https://github.com/thymikee/jest-preset-angular) for testing
- [Lerna](https://github.com/lerna/lerna) for multi packages
- eslint
- GitHub CI action to build, test, and release

## Checklist

You can use the prepare.ps1 script to bulk rename/replace "template-angular-package" to the repo folder name:

```
./prepare
```

Manual checklist:
- Replace "template-angular-package" in file and file names with your repo name
- Update LICENSE.txt
- Replace "Mohammad Rahhal"
- Add NPM_TOKEN GitHub secret for CI

## Used by

- https://github.com/mrahhal/ngx-chain-guards
