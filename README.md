# bfo-prismic-theme
Prismic theme contains the prismic custom-types shared by bfo users
Follow the instructions below to create a prismic repo for a new BFO instance

### prerequis
- create a new prismic account for the client
- create a new mail address or gmail alias for the client and add this email to the prismic users
- recommended node version 16.13.0

### install prismic cli 
    npm install -g prismic-cli

### run command to use theme and create the repo
the command should ask you to login prismic, then ask the name of the new prismic repo

    prismic theme --theme-url https://github.com/wizaplace/bfo-prismic-theme --conf prismic-configuration.json
    
### once the new repo is created
- visit https://prismic.io/dashboard and choose the new repo
- go to settings > API & security > generate an access token
- create the token and copy to env var PRISMIC_TOKEN
- update env var PRISMIC_URL to https://{name-of-new-repo}.prismic.io/api/v2
- go to settings > Translations & locales, setup as needed
- add 8 necessary documents (home, footer, header, notfound, landing_vendor, about_us, cookies), copy each doc for each locale, publish each doc


