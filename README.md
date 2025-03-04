![github-docs-banner](https://user-images.githubusercontent.com/74286884/156865155-7af481ea-261d-40ee-83b0-64e414072a22.png)

<p align="center" style="text-align: center;">
<a href="https://lbesson.mit-license.org">
  <img alt="MIT license"
       src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square"
       align="center">
</a>
<a href="https://twitter.com/intent/tweet?text=Git%20Connected%20%20https%3A%2F%2Fgithub.com%2Fwil-gerard%2Fgit-connected">
  <img alt="tweet"
       src="https://img.shields.io/twitter/url/https/github.com/ArmynC/ArminC-AutoExec.svg?style=flat-square&logo=twitter"
       target="_blank"
       align="center" />
</a>
  
# Git Connected

Git Connected is a social networking application that allows software engineers to reciprocate connections, follows, and endorsements - built by and for the [100Devs](https://leonnoel.com/100devs/) community.

## Table of Contents
* [Features](#features)
* [Tools and technologies](#tools-and-technologies)
* [Contributing :hearts:](#contributing)
* [Installation and local development](#installation-and-local-development)
* [Contributors](#contributors)
* [License](#license)

### Features
- Login through Discord OAuth first checks if a user is a part of the 100Devs server
- Connect your GitHub and Twitter accounts
- Update your username, location, and bio
- Follow other 100Devs directly in-app
- A featured 100Dev page

#### Made by and for the 100Devs community
User login that only allows members of the 100Devs Discord server.

![sign-in](https://user-images.githubusercontent.com/74286884/156219311-52e31316-2435-4e19-bbf0-981c30d9233d.gif)

#### Connect across Twitter, GitHub, and Discord
Follow other 100Devs and be followed on all platforms, directly in-app.

![follow](https://user-images.githubusercontent.com/74286884/156219385-920d9663-a2cd-4e8a-9e6f-f17cefcfb3f5.gif)

Future improvements:
- Users can add tags to their profiles (coffee chat, currently employed, looking for work, group project, etc.)
- User search by location and tags
- Group project forum where users can pin GitHub repos

### Tools and technologies

#### Frontend

  - [TypeScript](https://www.typescriptlang.org/)
  - [React](https://reactjs.org/)
  - [Axios](https://axios-http.com/)
  - [Tailwind CSS](https://tailwindcss.com/)
  - [Styled-components](https://styled-components.com/)
  - [Twin.macro](https://github.com/ben-rogerson/twin.macro)

#### Backend

  - [TypeScript](https://www.typescriptlang.org/)
  - [Node](https://nodejs.org/)
  - [Express](http://expressjs.com/)
  - [MongoDB](https://docs.mongodb.com/)
  - [Passport](https://www.passportjs.org/)
    - [Discord OAuth 2.0](https://github.com/nicholastay/passport-discord)
    - [GitHub OAuth 2.0](https://github.com/jaredhanson/passport-oauth2)
    - [Twitter OAuth 1.0a](https://github.com/jaredhanson/passport-twitter)

## Contributing 

Please check out the [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)

There are several ways to help.

1. **Spread the word:** More users means more people testing and contributing to the app which in turn means better stability and possibly more and better features. You can [tweet about it](https://twitter.com/intent/tweet?url=https%3A%2F%2Fgithub.com%2Fwil-gerard%2Fgit-connected&text=Hey%20folks%21%20We%20are%20building%20a%20social%20networking%20app%20to%20help%20connect%20the%20%23100devs%20community.%20Want%20to%20help%20out%3F&hashtags=techtwitter), share it on [LinkedIn](http://www.linkedin.com/shareArticle?mini=true&url=https://github.com/wil-gerard/git-connected&title=A%20social%20networking%20app%20to%20help%20connect%20the%20%23100devs%20community.), [reddit](http://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Fwil-gerard%2Fgit-connected&title=A%20social%20networking%20app%20to%20help%20connect%20the%20%23100devs%20community.) or any of your favorite social media platforms. Every little bit helps!

2. **Provide a Pull Request:** Here is a list of [the most popular community requests](https://github.com/wil-gerard/git-connected/issues?q=is%3Aissue+is%3Aopen+sort%3Areactions-%2B1-desc) and here's some info on [installation and setup](https://github.com/wil-gerard/git-connected#installation-and-setup).
   Please make sure that you're following the [angular commit guidelines](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#commits) and to also include the issue number in your commit message, if you're fixing a particular issue (e.g.: `test: create unit test for new user #44`).

3. **[Answer questions](https://github.com/wil-gerard/git-connected/discussions)**: You know the answer to another user's problem? Share your knowledge!

4. **[Provide your opinion](https://github.com/wil-gerard/git-connected/discussions?discussions_q=label%3A%22community+feedback+wanted%22):** Your input might be helpful even if it is just an up- or down-vote.

5. **[Provide a more refined ui spec for existing feature requests](https://github.com/wil-gerard/git-connected/issues?q=is%3Aissue+is%3Aopen+label%3A%22needs+concept+and%2For+ui+spec%22)**

6. **[Report bugs](https://github.com/wil-gerard/git-connected/issues/new)**

7. **[Make a feature or improvement request](https://github.com/wil-gerard/git-connected/issues/new)**: Something can be be done better? Something essential missing? Let us know!

8. **Design, project management, translations, etc.**: You don't have to be programmer to help!

## Installation and local development

These instructions will get a copy of the project on your local machine for development and testing purposes. If you have any further questions, feel free to reach out to [Wil Gerard.](https://github.com/wil-gerard)

### Prerequisites

* Node v16 or higher
* Yarn v3.2.0

### Installation and setup

For instructions on installing Node, please visit [https://nodejs.org/](https://nodejs.org/)

#### Installing Yarn 2 (aka Yarn Modern)
```
npm install -g yarn
yarn set version berry
```
#### Clone repo
```
git clone https://github.com/wil-gerard/git-connected.git
```
#### Install dependencies
```
yarn
```

#### Environment variables
- You will find a .env template at git-connected/server/.envTEMPLATE
- Delete "TEMPLATE" from the filename
- MONGODB_URL: Instructions on [setting up a MongoDB Atlas account.](https://hevodata.com/learn/mongodb-atlas-nodejs/) Refer to the image below on where to find your connection string.
  
  ![mongodb_url](https://user-images.githubusercontent.com/74286884/159807213-b7146a46-22e6-4927-bc18-65a2ed63025b.png)
- DISCORD_CLIENT_ID and DISCORD_SECRET: Instructions on [setting up a Discord OAuth application](https://circlertech.com/working-with-discord-oauth2) 
  - Redirect URI: `http://localhost:4000/api/auth/discord/callback`
  
*The previous two environment variables should be enough for most development adjustments. But if you'd like full app functionality, feel free to add the other environment variables.*

- TWITTER_CONSUMER_KEY and TWITTER_CONSUMER_SECRET: [Create a Twitter OAuth app with v1.1 access](https://developer.twitter.com)
  - Redirect URI: `http://localhost:4000/api/auth/twitter/callback`
- GITHUB_CLIENT_ID and GITHUB_CLIENT_SECRET: [Create a GitHub OAuth app](https://docs.github.com/en/developers/apps/building-oauth-apps/creating-an-oauth-app)
  - Redirect URI: `http://localhost:4000/api/auth/github/callback`

#### Developing locally

Open a terminal and run this script to start the dev server
```
yarn workspace server dev
```

In a new terminal, run this script to start the React client
```
yarn workspace client start
```

## Contributors
  - **Wil Gerard** - *Software Engineer* - [wil-gerard](https://github.com/wil-gerard)
  - **Ken aka Frosty** - *Software Engineer* - [KenAKAFrosty](https://github.com/KenAKAFrosty)
  - **Jeff Bucher** - *Software Engineer* - [JeffBucherDev](https://github.com/JeffBucherDev)
  - **Miracle Banks** - *Software Engineer* - [miraclebanks](https://github.com/miraclebanks)
  - **Dan Anderson** - *Software Engineer* - [DanCAnderson](https://github.com/DanCAnderson)
  - **Tim Jackson** - *Software Engineer* - [timjacksonm](https://github.com/timjacksonm)
  - **Gerard Strecker** - *Software Engineer* - [whoadood](https://github.com/whoadood)

See also the list of
[contributors](https://github.com/wil-gerard/GitConnected/contributors)
who participated in this project.

## License

MIT License - see the [LICENSE.md](LICENSE.md) file for details
