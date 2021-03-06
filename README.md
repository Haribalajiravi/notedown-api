# notedown-api

Fork || clone > `npm install` > `npm run dev-start` > Open link [http://localhost:3000/docs](http://localhost:3000/docs) in browser
## Overview
This project is entirely built on [Typescript](https://www.typescriptlang.org/docs/handbook/basic-types.html). Before developing go through [Best Practices](https://www.typescriptlang.org/docs/handbook/declaration-files/do-s-and-don-ts.html).

If trying to install new packages, make sure install it's types too. like `npm install --save-dev @types/<package_name>`. If you don't find @types, create types at `./src/types/<package_name>`.

### Packages used

- [express](https://expressjs.com/en/5x/api.html) - Server listener and REST standard can be maintainable via this package.
- [Joi](https://joi.dev/api/?v=17.3.0) - Payload validation as middleware
- [mongoose](https://mongoosejs.com/) - MongoDB accessor
- [swagger](https://swagger.io/docs/specification/basic-structure/): packs [[swagger-ui-express](https://www.npmjs.com/package/swagger-ui-express) - REST API, UI document specification, [swagger-jsdoc](https://www.npmjs.com/package/swagger-jsdoc) - Convert command-line specs as js schema towards swagger-ui-express]
- [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken) - Bearer Authentication token system
- [passport](http://www.passportjs.org/docs/authenticate/): packs [[passport-google-plus-token](https://www.npmjs.com/package/passport-google-plus-token), [passport-local](http://www.passportjs.org/packages/passport-local/), [passport-jwt](http://www.passportjs.org/packages/passport-jwt/)] - Authorization middleware

### Development packages
 - [nodemon](https://nodemon.io/) - Auto dev reloader
 - [tslint](https://palantir.github.io/tslint/) - To maintain code standards and avoid runtime errors prior. Install VS code extension [TSlint](https://marketplace.visualstudio.com/items?itemName=ms-vscode.vscode-typescript-tslint-plugin)
  - [prettier](https://prettier.io/) - Best code formatter. Install VS code extension [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  - [husky](https://typicode.github.io/husky/#/) - Git hooks, mainly used to linting code before commit.


Create a .env file for Dev setup
Try [Google Developer Console](https://console.developers.google.com/apis/credentials) to create a OAuth 2.0 Client ID to test Google OAuth2.
To create test access_token of Google OAuth2.0 try this [playground](https://developers.google.com/oauthplayground/)
```
MONGO_DB_URL=mongodb://localhost/notedown
ORIGIN=http://localhost:3000
JWT_SECRET=SomeSuperSecret
GOOGLE_CLIENT_ID=xxxxxxxxxxxxxxxxqa8mroqr1g.apps.googleusercontent.com
GOOGLE_CLIENT_SECRET=xxxxxxxxxxxxxx-Np
```
