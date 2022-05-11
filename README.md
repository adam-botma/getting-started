# getting-started
A quick guide to getting your new MacPro set up for dev


## Install Homebrew
1. Add xcode select: 

```xcode-select --install```

2. Install homebrew: 

```/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```

3. Run the following two commads to finish homebrew set up: 

```echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/adambotma/.zprofile``` 

```eval "$(/opt/homebrew/bin/brew shellenv)"```

4. Verify Homebrew was intalled correctly: 

``` brew help ``` 


Homebrew Docs : https://docs.brew.sh/  

## Install NVM 
1. Make sure you are in your root directory 

``` cd ~ ```

2. create a .zshrc file 
``` touch .zshrc ```

3. install NVM using curl

``` curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash ```

4. install node using NVM 

``` nvm install node ``` 
 - this will install the latest version on node 

5. install most active LTS (longer term support) version 

``` nvm install --lts ```

NVM Docs: https://github.com/nvm-sh/nvm


## Add Global npm packages

1. Nodemon 

``` npm install -g nodemon ``` 

2. Yarn 

``` npm install -g yarn ```


## Add Shopify CLI 

` brew tap shopify/shopify`

`  brew install shopify-cli `

Shopify CLI docs: https://shopify.dev/themes/tools/cli


## Add ngrok
1. Create an account here: https://dashboard.ngrok.com/get-started/setup
2. Install ngrok: 

```brew install --cask ngrok```

3. add your auth token (can be found here: https://dashboard.ngrok.com/get-started/your-authtoken)

```ngrok config add-authtoken [your auth token]```

```shopify app tunnel [your auth token]```


## To View Shopify CLI errors

add the following to your ```.zprofile``` in your root directory

```export SHOPIFY_CLI_STACKTRACE=1```


## Additional Items to Add
Postman:  ```brew install --cask postman```

React Chrome Devtools: https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi/related?hl=en
