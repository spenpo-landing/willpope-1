## A full stack implementation of the [spenpo-landing](https://www.npmjs.com/package/spenpo-landing) npm module built with Next.js

### env variables:

| Variable                           | Description                                                                                                                                                                                | Reqired |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |
| NEXT_PUBLIC_TITLE                  | CONTENT: title that appears at the top of the landing page                                                                                                                                 | yes     |
| NEXT_PUBLIC_NAME                   | CONTENT: name that appears below title                                                                                                                                                     | yes     |
| NEXT_PUBLIC_SUBTITLE               | CONTENT: subtitle that appears below the name                                                                                                                                              | yes     |
| NEXT_PUBLIC_ACTION_STATEMENT       | CONTENT: call to action that appears on the button below the subtitle. if not included, button will not appear                                                                             | no      |
| NEXT_PUBLIC_ACTION                 | CONTENT: relative or absolute url to be brought up in a new tab when call to action is clicked                                                                                             | no      |
| NEXT_PUBLIC_SOCIALS                | CONTENT: stringified json array of urls to social media profiles displayed at the bottom of the landing page                                                                               | no      |
| NEXT_PUBLIC_HEADSHOT               | CONTENT: relative or absolute url of the image displayed on the landing page                                                                                                               | yes     |
| NEXT_PUBLIC_BG_COLOR               | CONTENT: hex code for the background color of the landing page                                                                                                                             | no      |
| NEXT_PUBLIC_BG_IMAGE               | CONTENT: absolute url of the background image of the landing page                                                                                                                          | no      |
| NEXT_PUBLIC_ACCENT_COLOR           | CONTENT: hex code for the main color of the landing page. accents the call to action and social media buttons                                                                              | no      |
| NEXT_PUBLIC_SECONDARY_ACCENT_COLOR | CONTENT: hex code for the secondary color on hover effect of call to action and social media buttons                                                                                       | no      |
| NEXT_PUBLIC_HIDE_ADMIN             | boolean: hides the admin button from the top right corner. if true, the admin features can still be accessed by manually accessing the path /api/auth/signin                               | no      |
| NEXT_AUTH_USERNAME                 | username for accessing admin features                                                                                                                                                      | no      |
| NEXT_AUTH_PASSWORD                 | password for accessing admin features. [argon2](https://argon2.online/) hashed                                                                                                             | no      |
| NEXTAUTH_SECRET                    | [random string used to hash tokens](https://next-auth.js.org/configuration/options#secret). required in order to use admin features                                                        | no      |
| NEXTAUTH_URL                       | [canonical url of your site](https://next-auth.js.org/configuration/options#nextauth_url). automatically set to VERCEL_URL if deploying to Vercel. required in order to use admin features | no      |
| GH_TOKEN                           | [Github personal access token](https://github.com/settings/tokens). required for accessing Github in admin functions                                                                       | no      |
| VERCEL_TOKEN                       | [Vercel rest api token](https://vercel.com/account/tokens). required for accessing Vercel in admin functions                                                                               | no      |
| VERCEL_TEAM                        | id of your Vercel team if project is deployed to a team account                                                                                                                            | no      |
| NEXT_PUBLIC_PROJECT_NAME           | your Vercel project name. should be added after initial deployment if you plan to use the CMS feature                                                                                      | no      |