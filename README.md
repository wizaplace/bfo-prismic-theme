# _bfo-prismic-theme_
This repo contains the Prismic custom-types used by BFO instances.

Follow the instructions below to create a Prismic repo for a new BFO instance.

### Prerequisities
- Create a new Prismic account for the client.
- Create a new mail address or gmail alias for the client and add this email to the Prismic users list.
- Recommended Node version: 16.13.0.

### Install prismic cli 
    npm install -g prismic-cli

### Run the command to use a theme and create the repo
The command should ask you to login to Prismic, then ask the name of the new prismic repo

    prismic theme --theme-url https://github.com/wizaplace/bfo-prismic-theme --conf prismic-configuration.json
    
### Once the new repo is created
- Visit https://prismic.io/dashboard and choose the new repo.
- Go to settings > API & security > generate an access token.
- Create the token and copy it to the env var PRISMIC_TOKEN.
- Update the env var PRISMIC_URL to https://{name-of-new-repo}.prismic.io/api/v2
- Go to settings > Translations & locales, setup as needed.
- Add the 8 necessary documents (home, footer, header, notfound, landing_vendor, about_us, cookies), then copy each doc for each locale, and finally publish each of them.


