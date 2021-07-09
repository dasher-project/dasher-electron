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

# Third Party

## MozoLM
To enable and start the micro-service, you must have have Docker installed.
Steps 1 and 2 can be triggered by a script via `npm start`:

0. Define Training File
1. Start the Envoy Proxy
2. Start the MozoLM service

```
git clone https://github.com/google-research/mozolm
export TRAINING_FILE=mozolm/mozolm/models/testdata/en_wiki_1Kline_sample.txt
cp $TRAINING_FILE ~/training.txt
cd submodules/dasher-web/browser/dasher/third_party/mozolm
npm install
npm start
```
