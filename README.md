[![Build/release](https://github.com/dasher-project/dasher-electron/actions/workflows/build.yml/badge.svg)](https://github.com/dasher-project/dasher-electron/actions/workflows/build.yml)
[![CI](https://github.com/dasher-project/dasher-electron/actions/workflows/lint.yml/badge.svg)](https://github.com/dasher-project/dasher-electron/actions/workflows/lint.yml)

# Dasher Electron

Electron distribution of the Dasher application.
For latest releases see [here](https://github.com/dasher-project/dasher-electron/releases/latest)

# Running Locally

## Clone this repository and make it your working path.
`git clone git@github.com:dasher-project/dasher-electron.git`

`cd dasher-electron`

## Initialize subrepositories.
`git submodule update --init`

## Install dependencies.
`yarn install`

## Run the application.
`yarn start`

## Locally build host binary.

`yarn build`

# Production Builds

Production builds are periodically realeased for the following platforms:

1. Windows (.exe)
2. Mac (.dmg)
3. Linux (.AppImage)

For more information on running AppImage files, please see (https://docs.appimage.org/user-guide/faq.html)

## Creating a Production Build

To create a new production build:
1. Merge the feature branches required into main
2. Update the version number within package.json
3. Tag the commit with the corresponding version number and push the changes to origin.

Example:

```
package.json
...
  "version": "1.1.2",
...

git tag v1.1.2
git push && git push --tags
```

## Versioning

Dasher-Electron follows [Symantic Versioning](https://semver.org/)
