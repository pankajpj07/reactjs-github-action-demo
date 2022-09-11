
# lb-ui-components

  ## Tools You Might Need
  1. Version Control System - [git](https://git-scm.com/downloads) 
  2. Package Manager - [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) or [yarn](https://classic.yarnpkg.com/lang/en/docs/install/#windows-stable)
  3. Code Editor - [VsCode](https://code.visualstudio.com/download) (recommended)
  4. Runtime - [NodeJS](https://nodejs.org)
  5. Node version manager - [nvm for windows](https://github.com/coreybutler/nvm-windows) - [nvm for mac](https://tecadmin.net/install-nvm-macos-with-homebrew)
  6. AWS CLI - [aws cli installation guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
  

## ~Installation and Setup Guide:

1. [clone repository](#clone-repository) : This will clone your repository in local machine.
2. [installation and setup](#installation-and-setup) : This step will help you setting up the environment.
3. [Installing node module](#installing-node-modules): This step will install/add all the packages required.
4. [running storybook](#running-storybook): This step will build storybook of all the custom components and run it on the browser.

If you face any errors, refer to [common error's guide](#common-errors-guide)

  

### clone repository

  

```sh
git clone https://github.com/MyRetailCare/lb-ui-components.git
cd lb-ui-components
```

### installation and setup

 

Since we will be using aws command within this project. It's better to install aws cli.

You can refer to [aws cli installation guide](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

  
#### npm run prepare
After successful aws cli installation, run the below command:
```sh
npm run prepare
```

This command will run **aws codeartifact login --tool npm --repository lb-ui-components --domain legalbuddy**
 

If you face any .npmrc or legalbuddy file not found error. you can run below commands in terminal via Run as administrator mode (Windows cmd) 

```sh
npm install -g npmrc
npmrc -c legalbuddy
npmrc legalbuddy
```
now try running the [npm run prepare](#npm-run-prepare) and when it runs successfully, authenticate with below details:
```sh
> AWS Access Key ID: <Wil be given>
> AWS Secret Access key: <Wil be given>
> Default Region Name: <Will be given, as it varies>
> Default Output Format: json
```
## installing node modules

```sh
npm install
```

## running storybook
```sh
npm run storybook
```
If you face any errors, refer to [common error's guide](#common-errors-guide)
## common errors guide
###### [NPM ERR Code E401: Unable to authenticate, need: Bearer authorization](https://stackoverflow.com/questions/59894644/npm-err-code-e401-unable-to-authenticate-need-bearer-authorization)
##### [issue-with-publishing-npm-package-org-couchdb-userusername-is-not-in-the-npm](https://stackoverflow.com/questions/67514615/issue-with-publishing-npm-package-org-couchdb-userusername-is-not-in-the-npm)
 
