# Dasher Electron

Electron distribution of the Dasher application.

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

To create a new production build, update the version number within package.json and then tag the commit with the corresponding version.

Example:

```
package.json
...
  "version": "1.1.2",
...

git tag v1.1.2
```
