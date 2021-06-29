# Dasher Electron

Electron distribution of the Dasher application.

# Running Locally

## Clone this repository and make it your working path.
`git clone git@github.com:dasher-project/dasher-electron.git`
`cd dasher-electron`

## Initialize subrepositories.
`git submodule update --init`

## Install dependencies.
`npm install`

## Run the application.
`npm start`


## Building Targets

# Mac OS

1. Install brew if you don't have it already
2. brew install fakeroot and dpkg
3. brew install mono and wine-stable
4. npm i -g @electron-forge/cli
5. npm run make --platform=darwin

NOTE: The first time building with wine may require additional installs, simply follow the wizard.
