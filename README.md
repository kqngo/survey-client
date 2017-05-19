[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)


## Project Links

#### Back-End Deplpyed
[ProjectApiDeployed](https://floating-savannah-15725.herokuapp.com/)
#### Back-End Repo
[ProjectApiRepo](https://github.com/push-it-real-good/survey-express-api)

#### Front-End Deployed
[ProjectClientDeployed](https://push-it-real-good.github.io/survey-client/)
#### Front-End Repo
[ProjectClientRepo](https://github.com/push-it-real-good/survey-client)

## ERD

<img width="799" alt="survey-erd" src="https://cloud.githubusercontent.com/assets/26236941/26231974/bb4ca918-3c20-11e7-844a-637122c5ce98.png">

## Wireframe

![wireframe](https://cloud.githubusercontent.com/assets/26236941/26231973/b82e73ba-3c20-11e7-95ce-a75672ef1642.png)

## User Stories

1. As a surveyor, I want to sign up, so that I can create surveys.
2. As a surveyor, I want to sign in, so that I can create surveys.
3. As a surveyor, I want to change a password so that I can protect my identity.
4. As a surveyor, I want to sign out, so that I can safely log out and no one can see my survey data.
5. As a surveyor, I want to create a survey and generate a link to each survey.
6. As a surveyor, I want to update existing surveys so that I can modify them.
7. As a surveyor, I want to delete a survey if it is no longer needed.
8. As a surveyor, I want to be able to view all results of a survey in a dashboard.
9. As a respondent, I want to be able to fill out the survey.
10.As a respondent, I want to be able to submit the survey.


# browser-template

A template for starting front-end projects. Webpack for `require` system, build
pipeline, and development server. Boostrap and Handlebars.js included. No
front-end frameworks included.

## Dependencies

Install with `npm install`.

-   [Webpack](https://webpack.github.io)
-   [Bootstrap](http://getbootstrap.com)
-   [Handlebars.js](http://handlebarsjs.com)

At the beginning of each cohort, update the versions in
[`package.json`](package.json) by replace all versions with a glob (`*`) and
running `npm update --save && npm update --save-dev`. You may wish to test these
changes by deleting the `node_modules` directory and running `npm install`.
Fix any conflicts.

## Installation

1.  [Download](../../archive/master.zip) this template.
1.  Unzip and rename the template directory.
1.  Empty [`README.md`](README.md) and fill with your own content.
1.  Move into the new project and `git init`.
1.  Install dependencies with `npm install`.

## Structure

Dependencies are stored in [`package.json`](package.json).

Do not configure `grunt` packages directly in the
[`Gruntfile.js`](Gruntfile.js). Instead, store configurations in the
[`grunt`](grunt) directory. You won't need a top-level key, since that's
generated by the `Gruntfile.js` based on the filename of the configuration
object stored in the `grunt` directory.

Developers should store JavaScript files in [`assets/scripts`](assets/scripts).
The "manifest" or entry-point is
[`assets/scripts/index.js`](assets/scripts/index.js). In general, only
application initialization goes in this file. It's normal for developers to
start putting all code in this file, but encourage them to break out different
responsibilities and use the `require` syntax put references where they're
needed.

Developers should set `config.apiOrigins.production` (and
`config.apiOrigins.development` if it differs from the default).  With
`apiOrigins` set, developers may rely on `config.apiOrigin` as the base for API
URLs.

Developers should store styles in [`assets/styles`](assets/styles) and load them
from [`assets/styles/index.scss`](assets/styles/index.scss).

Developers should use [getFormFields](forms.md) to retrieve form data to send to
an API.

To deploy a browser-template based SPA, run `grunt deploy`.

## Tasks

Developers should run these often!

-   `grunt nag` or just `grunt`: runs code quality analysis tools on your code
    and complains
-   `grunt reformat`: reformats all your code in a standard style
-   `grunt <server|serve|s>`: generates bundles, watches, and livereloads
-   `grunt test`: runs any automated tests, depends on `grunt build`
-   `grunt build`: place bundled styles and scripts where `index.html` can find
    them

## [License](LICENSE)

1.  All content is licensed under a CC­BY­NC­SA 4.0 license.
1.  All software code is licensed under GNU GPLv3. For commercial use or
    alternative licensing, please contact legal@ga.co.
