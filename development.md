# The development environment

I am using a macMini M2 with OSX.

## Install NodeJS

```bash
brew install node@18
```

You need to add the following to the end of your `~/.zshrc` file:

```bash
export PATH="/opt/homebrew/opt/node@18/bin:$PATH"
export LDFLAGS="-L/opt/homebrew/opt/node@18/lib"
export CPPFLAGS="-I/opt/homebrew/opt/node@18/include"
```

Then `source ~/.zshrc` or logout and login again.

## Install yarn

```bash
npm install -g yarn
```

## Clone the boilerplate repo

```bash
git clone https://github.com/niftyz-learn/smartcontract-boilerplate.git
cd smartcontract-boilerplate
```

## yarn network
Start a new terminal (tab or window) and start the network:

```bash
yarn network
```

Then go back to the other terminal and continue.

## hardhat

```bash
yarn task deploy hardhat
```
