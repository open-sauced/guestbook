# THE OPENSAUCED GUESTBOOK

This guestbook is a place for people who have taken [OpenSauced](https://opensauced.pizza)'s [Intro to Open Source course](https://github.com/open-sauced/intro) to take their first steps into contributing to open source.

## Getting Started

First, you'll want to have Node.js installed. You can do this by going to [nodejs.org](https://nodejs.org) and downloading the latest version. Then, follow these steps:

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository) this repository.
2. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository#cloning-a-repository) your forked repository to your computer.
3. Run `npm install` to install the dependencies.
4. Create a new branch.

   The best practice for open-source contributors to work on changes is in a new branch to isolate them from the `main` branch.

   Run this command on your terminal to create a new branch. You can name the branch anything you want.

   ```bash
   git checkout -b branch-name
   ```

5. Add yourself to the guestbook.

   There are two ways you can complete this activity:

   - Using the CLI tool.
   - Manually editing the `.all-contributorsrc` file

   Although adding yourself to the guestbook with the CLI tool is simpler, we recommend you to manually editing the file to get more experience adding and committing your changes, creating pull requests and pull request reviews. Below, you'll find the directions for each method:

   **CLI Tool**

   - Run `npm run contributors:add` in your terminal.

     Follow the instructions to add yourself to the guestbook. After you finish and click enter, you must click enter again to confirm your choices.

   **Manual Addition**

   - Open the `.all-contributorsrc` file.
   - Go to the last contributor in the contributors array.
   - Add a comma after the last closing curly bracket ( `},` ).
   - Copy and paste the template below:

     ```javascript
     {
        "login": "",
        "name": "",
        "avatar_url": "",
        "profile": "",
        "contributions": []
     }
     ```

   - Add yourself manually to the guestbook by updating this information:

     - **login**: Your GitHub's username.
     - **name**: Your name.
     - **avatar_url**: URL to your avatar on GitHub.

       In your browser, copy and paste the link of your GitHub profile, append `.png` at the end — for example, `https://github.com/USER_NAME.png` — and click enter. Copy and paste the link here.

     - **profile**: Link to your website (if you include it in your GitHub profile) **or** your GitHub profile.
     - **contribution**: Type of your contributions.

       Refer to the type (in the first column) in this [emoji key and contribution types](https://allcontributors.org/docs/en/emoji-key) to fill this value.

       The result would be like this:

       ```javascript
       {
         "login": "github-username",
         "name": "User Name",
         "avatar_url": "https://avatars.githubusercontent.com/u/xxxxxxxx?v=x",
         "profile": "URL link",
         "contributions": [
         "question",
         "blog",
         "code"
         ]
       }
       ```

     _Remember to add a comma after the quotes, except for the last one in the array and the last closing curly bracket_.

6. Run `npm run contributors:generate` in your terminal to generate the guestbook on the README.

7. If you used the CLI tool method in step 6, to add yourself to the guestbook, **skip this step;** otherwise:
   Add and commit your changes by running this command:

   ```bash
   git commit -am "Your message"
   ```

   Change `"Your message"` to your own message. For example, `"Add Alice to the guestbook"`.

8. Run `git log` to check if you have committed your changes. Press `Q` to close the log.

   If you add yourself using the CLI tool, it automatically adds and commits your changes. So you will see this automated commit message:

   ```bash
   docs: add @your_username as a contributor
   ```

9. Push the commit to your forked repository with this command:

   ```bash
   git push -u origin branch-name
   ```

10. Go to your forked repository on GitHub and [create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork) with the title `feat: add {GitHub username} as a contributor`.

## Keeping Branch Up to Date and Resolving Merge Conflicts

Merge conflicts are something you'll commonly encounter when contributing to an open source project. They usually occur when there are changes on the same line(s) in the same file(s) from two different branches.

Since the main purpose of the guestbook is to add your name to `.all-contributorsrc` and the `README.md` files, there is a high chance that you will encounter merge conflicts that you need to resolve before your pull request (PR) can be merged. It happens when maintainers have merged PRs before yours while you're working on your changes or waiting for your PR to be reviewed.

In this section, we will walk you through how to keep your branch up to date and how to resolve conflicts for this project.

### Keeping Branch Up to Date

Before resolving conflicts, your branch has to be in sync with the latest changes in the `main` branch of the original (`upstream`) repository.

First, you must update your forked (`origin`) repository:

1. Go to your forked repository on GitHub.
2. Click the "Sync fork" button.
3. Click the green "Update branch" button.

Then, pull the latest changes in the `main` branch in the `origin` repository to your local working branch by following these steps in your terminal:

1. Go to your working branch.

   ```bash
   git checkout <your-branch-name>
   ```

2. Pull the latest changes with this command:

   ```bash
   git pull origin main
   ```

### Resolving Merge Conflicts

Follow these steps to resolve the merge conflicts:

1. In the `.all-contributorsrc` file:

   - Click the "Accept Both Change" option on the top of your workspace in VSCode.
   - Move your profile details to the end of the contributors array and fix anything necessary.

2. In the `README.md` file:

   - Click the "Accept Incoming Change" option on the top of your workspace in VSCode for each conflict in this file.

3. Run `npm run contributors:generate`.

   You will now see that the all contributors badge has been incremented, and your profile is generated at the end of the contributors list in the `README.md` file.

4. Add and commit your changes.

   ```bash
   git commit -am "Resolve merge conflicts"
   ```

5. Push your commits to your remote branch.

   ```bash
   git push
   ```

Congratulations on your first contribution! 🎉

## What's Next?

You can add this contribution to your [OpenSauced](https://opensauced.pizza) resume and profile as [outlined in the course](https://github.com/open-sauced/intro/blob/main/05-how-to-contribute-to-open-source.md).

Hungry for more contributions? Check out our [pizza verse](https://github.com/open-sauced/pizza) repository and join us in celebrating pizza!🍕😄

---

## 🤝 Contributing

All contributors are required to abide by our [Code of Conduct](https://github.com/open-sauced/.github/blob/main/CODE_OF_CONDUCT.md). Please follow the Readme directions for contributing.
- **Translations:** If you want to translate the README and other necessary parts of this repo, check out our community guidelines.
 

## Contributors

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-62-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://tej.as/"><img src="https://github.com/tejasq.png?s=100" width="100px;" alt="Tejas Kumar"/><br /><sub><b>Tejas Kumar</b></sub></a><br /></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/pszymaniec"><img src="https://avatars.githubusercontent.com/u/102276661?v=4?s=100" width="100px;" alt="pszymaniec"/><br /><sub><b>pszymaniec</b></sub></a><br /><a href="#blog-pszymaniec" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=pszymaniec" title="Code">💻</a> <a href="#content-pszymaniec" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=pszymaniec" title="Documentation">📖</a> <a href="#example-pszymaniec" title="Examples">💡</a> <a href="#research-pszymaniec" title="Research">🔬</a> <a href="#translation-pszymaniec" title="Translation">🌍</a> <a href="#tutorial-pszymaniec" title="Tutorials">✅</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Apszymaniec" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://bekahhw.github.io/"><img src="https://avatars.githubusercontent.com/u/34313413?v=4?s=100" width="100px;" alt="BekahHW"/><br /><sub><b>BekahHW</b></sub></a><br /><a href="#question-BekahHW" title="Answering Questions">💬</a> <a href="#audio-BekahHW" title="Audio">🔊</a> <a href="#blog-BekahHW" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=BekahHW" title="Code">💻</a> <a href="#content-BekahHW" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=BekahHW" title="Documentation">📖</a> <a href="#eventOrganizing-BekahHW" title="Event Organizing">📋</a> <a href="#example-BekahHW" title="Examples">💡</a> <a href="#ideas-BekahHW" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-BekahHW" title="Mentoring">🧑‍🏫</a> <a href="#projectManagement-BekahHW" title="Project Management">📆</a> <a href="#promotion-BekahHW" title="Promotion">📣</a> <a href="#research-BekahHW" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3ABekahHW" title="Reviewed Pull Requests">👀</a> <a href="#talk-BekahHW" title="Talks">📢</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=BekahHW" title="Tests">⚠️</a> <a href="#tutorial-BekahHW" title="Tutorials">✅</a> <a href="#video-BekahHW" title="Videos">📹</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ValarieOyieke"><img src="https://avatars.githubusercontent.com/u/99278182?v=4?s=100" width="100px;" alt="ValarieOyieke"/><br /><sub><b>ValarieOyieke</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3AValarieOyieke" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ValarieOyieke" title="Code">💻</a> <a href="#example-ValarieOyieke" title="Examples">💡</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AValarieOyieke" title="Reviewed Pull Requests">👀</a> <a href="#userTesting-ValarieOyieke" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/shirenekboyd"><img src="https://avatars.githubusercontent.com/u/89878197?v=4?s=100" width="100px;" alt="Shirene Kadkhodai Boyd"/><br /><sub><b>Shirene Kadkhodai Boyd</b></sub></a><br /><a href="#a11y-shirenekboyd" title="Accessibility">️️️️♿️</a> <a href="#question-shirenekboyd" title="Answering Questions">💬</a> <a href="#blog-shirenekboyd" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Ashirenekboyd" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=shirenekboyd" title="Code">💻</a> <a href="#content-shirenekboyd" title="Content">🖋</a> <a href="#data-shirenekboyd" title="Data">🔣</a> <a href="#design-shirenekboyd" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=shirenekboyd" title="Documentation">📖</a> <a href="#ideas-shirenekboyd" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-shirenekboyd" title="Maintenance">🚧</a> <a href="#mentoring-shirenekboyd" title="Mentoring">🧑‍🏫</a> <a href="#plugin-shirenekboyd" title="Plugin/utility libraries">🔌</a> <a href="#research-shirenekboyd" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Ashirenekboyd" title="Reviewed Pull Requests">👀</a> <a href="#talk-shirenekboyd" title="Talks">📢</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=shirenekboyd" title="Tests">⚠️</a> <a href="#tool-shirenekboyd" title="Tools">🔧</a> <a href="#userTesting-shirenekboyd" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://www.shelleymcq.dev/"><img src="https://avatars.githubusercontent.com/u/81432121?v=4?s=100" width="100px;" alt="Shelley McHardy"/><br /><sub><b>Shelley McHardy</b></sub></a><br /><a href="#question-shelleymcq" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=shelleymcq" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=shelleymcq" title="Documentation">📖</a> <a href="#eventOrganizing-shelleymcq" title="Event Organizing">📋</a> <a href="#mentoring-shelleymcq" title="Mentoring">🧑‍🏫</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Ashelleymcq" title="Reviewed Pull Requests">👀</a> <a href="#tutorial-shelleymcq" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jmslynn"><img src="https://avatars.githubusercontent.com/u/72352820?v=4?s=100" width="100px;" alt="jmslynn"/><br /><sub><b>jmslynn</b></sub></a><br /><a href="#a11y-jmslynn" title="Accessibility">️️️️♿️</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=jmslynn" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://adiati.com/"><img src="https://avatars.githubusercontent.com/u/45172775?v=4?s=100" width="100px;" alt="Ayu Adiati"/><br /><sub><b>Ayu Adiati</b></sub></a><br /><a href="#question-adiati98" title="Answering Questions">💬</a> <a href="#blog-adiati98" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=adiati98" title="Code">💻</a> <a href="#content-adiati98" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=adiati98" title="Documentation">📖</a> <a href="#example-adiati98" title="Examples">💡</a> <a href="#mentoring-adiati98" title="Mentoring">🧑‍🏫</a> <a href="#talk-adiati98" title="Talks">📢</a> <a href="#translation-adiati98" title="Translation">🌍</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/droffilc1"><img src="https://avatars.githubusercontent.com/u/97587370?v=4?s=100" width="100px;" alt="Clifford Mapesa"/><br /><sub><b>Clifford Mapesa</b></sub></a><br /><a href="#a11y-droffilc1" title="Accessibility">️️️️♿️</a> <a href="#tutorial-droffilc1" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/edgarefigueroa"><img src="https://avatars.githubusercontent.com/u/55363462?v=4?s=100" width="100px;" alt="Edgar Figueroa"/><br /><sub><b>Edgar Figueroa</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=edgarefigueroa" title="Code">💻</a> <a href="#data-edgarefigueroa" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=edgarefigueroa" title="Documentation">📖</a> <a href="#research-edgarefigueroa" title="Research">🔬</a> <a href="#security-edgarefigueroa" title="Security">🛡️</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=edgarefigueroa" title="Tests">⚠️</a> <a href="#translation-edgarefigueroa" title="Translation">🌍</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/macabonilas827"><img src="https://avatars.githubusercontent.com/u/134240236?v=4?s=100" width="100px;" alt="Mark Anel Cabonilas"/><br /><sub><b>Mark Anel Cabonilas</b></sub></a><br /><a href="#a11y-macabonilas827" title="Accessibility">️️️️♿️</a> <a href="#question-macabonilas827" title="Answering Questions">💬</a> <a href="#blog-macabonilas827" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=macabonilas827" title="Code">💻</a> <a href="#data-macabonilas827" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=macabonilas827" title="Documentation">📖</a> <a href="#ideas-macabonilas827" title="Ideas, Planning, & Feedback">🤔</a> <a href="#tool-macabonilas827" title="Tools">🔧</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/deisenhut"><img src="https://avatars.githubusercontent.com/u/11063252?v=4?s=100" width="100px;" alt="Dan Eisenhut"/><br /><sub><b>Dan Eisenhut</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=deisenhut" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JayRKyd"><img src="https://avatars.githubusercontent.com/u/63754188?v=4?s=100" width="100px;" alt="Jay Knowles"/><br /><sub><b>Jay Knowles</b></sub></a><br /><a href="#blog-JayRKyd" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=JayRKyd" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://biroue.tech/"><img src="https://avatars.githubusercontent.com/u/27910604?v=4?s=100" width="100px;" alt="BIROUE ISAAC"/><br /><sub><b>BIROUE ISAAC</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=biroue10" title="Code">💻</a> <a href="#translation-biroue10" title="Translation">🌍</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Muyixone"><img src="https://avatars.githubusercontent.com/u/66142660?v=4?s=100" width="100px;" alt="Alarezomo Osamuyi"/><br /><sub><b>Alarezomo Osamuyi</b></sub></a><br /><a href="#a11y-Muyixone" title="Accessibility">️️️️♿️</a> <a href="#audio-Muyixone" title="Audio">🔊</a> <a href="#mentoring-Muyixone" title="Mentoring">🧑‍🏫</a> <a href="#userTesting-Muyixone" title="User Testing">📓</a> <a href="#question-Muyixone" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Muyixone" title="Tests">⚠️</a> <a href="#translation-Muyixone" title="Translation">🌍</a> <a href="#talk-Muyixone" title="Talks">📢</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/SushiJ"><img src="https://avatars.githubusercontent.com/u/74211783?v=4?s=100" width="100px;" alt="Sushant Sharma"/><br /><sub><b>Sushant Sharma</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=SushiJ" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/alishata/"><img src="https://avatars.githubusercontent.com/u/22107238?v=4?s=100" width="100px;" alt="Ali Shata"/><br /><sub><b>Ali Shata</b></sub></a><br /><a href="#blog-alishata128" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=alishata128" title="Code">💻</a> <a href="#content-alishata128" title="Content">🖋</a> <a href="#data-alishata128" title="Data">🔣</a> <a href="#design-alishata128" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=alishata128" title="Documentation">📖</a> <a href="#eventOrganizing-alishata128" title="Event Organizing">📋</a> <a href="#example-alishata128" title="Examples">💡</a> <a href="#ideas-alishata128" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-alishata128" title="Promotion">📣</a> <a href="#research-alishata128" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Aalishata128" title="Reviewed Pull Requests">👀</a> <a href="#talk-alishata128" title="Talks">📢</a> <a href="#tutorial-alishata128" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://ananfito.hashnode.dev/"><img src="https://avatars.githubusercontent.com/u/81890820?v=4?s=100" width="100px;" alt="Anthony Nanfito"/><br /><sub><b>Anthony Nanfito</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ananfito" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://kinhong.vercel.app/"><img src="https://avatars.githubusercontent.com/u/59541661?v=4?s=100" width="100px;" alt="Kin NG"/><br /><sub><b>Kin NG</b></sub></a><br /><a href="#blog-k1nho" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Ak1nho" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=k1nho" title="Code">💻</a> <a href="#design-k1nho" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=k1nho" title="Documentation">📖</a> <a href="#infra-k1nho" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Ak1nho" title="Reviewed Pull Requests">👀</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/zh-hadi"><img src="https://avatars.githubusercontent.com/u/108709174?v=4?s=100" width="100px;" alt="zh-hadi"/><br /><sub><b>zh-hadi</b></sub></a><br /><a href="#a11y-zh-hadi" title="Accessibility">️️️️♿️</a> <a href="#question-zh-hadi" title="Answering Questions">💬</a> <a href="#audio-zh-hadi" title="Audio">🔊</a> <a href="#blog-zh-hadi" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Azh-hadi" title="Bug reports">🐛</a> <a href="#business-zh-hadi" title="Business development">💼</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=zh-hadi" title="Code">💻</a> <a href="#content-zh-hadi" title="Content">🖋</a> <a href="#data-zh-hadi" title="Data">🔣</a> <a href="#design-zh-hadi" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=zh-hadi" title="Documentation">📖</a> <a href="#example-zh-hadi" title="Examples">💡</a> <a href="#financial-zh-hadi" title="Financial">💵</a> <a href="#ideas-zh-hadi" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-zh-hadi" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-zh-hadi" title="Maintenance">🚧</a> <a href="#mentoring-zh-hadi" title="Mentoring">🧑‍🏫</a> <a href="#platform-zh-hadi" title="Packaging/porting to new platform">📦</a> <a href="#plugin-zh-hadi" title="Plugin/utility libraries">🔌</a> <a href="#projectManagement-zh-hadi" title="Project Management">📆</a> <a href="#promotion-zh-hadi" title="Promotion">📣</a> <a href="#research-zh-hadi" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Azh-hadi" title="Reviewed Pull Requests">👀</a> <a href="#security-zh-hadi" title="Security">🛡️</a> <a href="#talk-zh-hadi" title="Talks">📢</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=zh-hadi" title="Tests">⚠️</a> <a href="#tool-zh-hadi" title="Tools">🔧</a> <a href="#translation-zh-hadi" title="Translation">🌍</a> <a href="#tutorial-zh-hadi" title="Tutorials">✅</a> <a href="#userTesting-zh-hadi" title="User Testing">📓</a> <a href="#video-zh-hadi" title="Videos">📹</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Axfez"><img src="https://avatars.githubusercontent.com/u/92069466?v=4?s=100" width="100px;" alt="Santiago Montoya Rendón"/><br /><sub><b>Santiago Montoya Rendón</b></sub></a><br /><a href="#question-Axfez" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Axfez" title="Code">💻</a> <a href="#data-Axfez" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Axfez" title="Documentation">📖</a> <a href="#maintenance-Axfez" title="Maintenance">🚧</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ATREAY"><img src="https://avatars.githubusercontent.com/u/66585295?v=4?s=100" width="100px;" alt="Atreay  Kukanur"/><br /><sub><b>Atreay  Kukanur</b></sub></a><br /><a href="#question-ATREAY" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ATREAY" title="Code">💻</a> <a href="#content-ATREAY" title="Content">🖋</a> <a href="#design-ATREAY" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ATREAY" title="Documentation">📖</a> <a href="#eventOrganizing-ATREAY" title="Event Organizing">📋</a> <a href="#ideas-ATREAY" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-ATREAY" title="Promotion">📣</a> <a href="#research-ATREAY" title="Research">🔬</a> <a href="#userTesting-ATREAY" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://leetcode.com/Suldana/"><img src="https://avatars.githubusercontent.com/u/114906181?v=4?s=100" width="100px;" alt="Ms. Suldana"/><br /><sub><b>Ms. Suldana</b></sub></a><br /><a href="#a11y-Suldana" title="Accessibility">️️️️♿️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/prabhatisme"><img src="https://avatars.githubusercontent.com/u/29323125?v=4?s=100" width="100px;" alt="Prabhat Bhagel"/><br /><sub><b>Prabhat Bhagel</b></sub></a><br /><a href="#audio-prabhatisme" title="Audio">🔊</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=prabhatisme" title="Code">💻</a> <a href="#design-prabhatisme" title="Design">🎨</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/kelvinyelyen"><img src="https://avatars.githubusercontent.com/u/52675327?v=4?s=100" width="100px;" alt="Kelvin Yelyen"/><br /><sub><b>Kelvin Yelyen</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=kelvinyelyen" title="Code">💻</a> <a href="#content-kelvinyelyen" title="Content">🖋</a> <a href="#design-kelvinyelyen" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Akelvinyelyen" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=kelvinyelyen" title="Documentation">📖</a> <a href="#ideas-kelvinyelyen" title="Ideas, Planning, & Feedback">🤔</a> <a href="#projectManagement-kelvinyelyen" title="Project Management">📆</a> <a href="#research-kelvinyelyen" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=kelvinyelyen" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Fatima-Abdirashid"><img src="https://avatars.githubusercontent.com/u/140537915?v=4?s=100" width="100px;" alt="Fatima-Abdirashid"/><br /><sub><b>Fatima-Abdirashid</b></sub></a><br /><a href="#a11y-Fatima-Abdirashid" title="Accessibility">️️️️♿️</a> <a href="#question-Fatima-Abdirashid" title="Answering Questions">💬</a> <a href="#audio-Fatima-Abdirashid" title="Audio">🔊</a> <a href="#blog-Fatima-Abdirashid" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3AFatima-Abdirashid" title="Bug reports">🐛</a> <a href="#business-Fatima-Abdirashid" title="Business development">💼</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Fatima-Abdirashid" title="Code">💻</a> <a href="#content-Fatima-Abdirashid" title="Content">🖋</a> <a href="#data-Fatima-Abdirashid" title="Data">🔣</a> <a href="#design-Fatima-Abdirashid" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Fatima-Abdirashid" title="Documentation">📖</a> <a href="#eventOrganizing-Fatima-Abdirashid" title="Event Organizing">📋</a> <a href="#example-Fatima-Abdirashid" title="Examples">💡</a> <a href="#financial-Fatima-Abdirashid" title="Financial">💵</a> <a href="#fundingFinding-Fatima-Abdirashid" title="Funding Finding">🔍</a> <a href="#ideas-Fatima-Abdirashid" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-Fatima-Abdirashid" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-Fatima-Abdirashid" title="Maintenance">🚧</a> <a href="#mentoring-Fatima-Abdirashid" title="Mentoring">🧑‍🏫</a> <a href="#research-Fatima-Abdirashid" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AFatima-Abdirashid" title="Reviewed Pull Requests">👀</a> <a href="#security-Fatima-Abdirashid" title="Security">🛡️</a> <a href="#talk-Fatima-Abdirashid" title="Talks">📢</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Fatima-Abdirashid" title="Tests">⚠️</a> <a href="#tool-Fatima-Abdirashid" title="Tools">🔧</a> <a href="#translation-Fatima-Abdirashid" title="Translation">🌍</a> <a href="#tutorial-Fatima-Abdirashid" title="Tutorials">✅</a> <a href="#userTesting-Fatima-Abdirashid" title="User Testing">📓</a> <a href="#video-Fatima-Abdirashid" title="Videos">📹</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Iqra-Issack"><img src="https://avatars.githubusercontent.com/u/140454697?v=4?s=100" width="100px;" alt="Iqra-Issack"/><br /><sub><b>Iqra-Issack</b></sub></a><br /><a href="#infra-Iqra-Issack" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-Iqra-Issack" title="Maintenance">🚧</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Muniir1"><img src="https://avatars.githubusercontent.com/u/121073318?v=4?s=100" width="100px;" alt="muniir1"/><br /><sub><b>muniir1</b></sub></a><br /><a href="#a11y-Muniir1" title="Accessibility">️️️️♿️</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/anyanime"><img src="https://avatars.githubusercontent.com/u/58043661?v=4?s=100" width="100px;" alt="Anyanime Benson"/><br /><sub><b>Anyanime Benson</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=anyanime" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=anyanime" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/IbnuAlii"><img src="https://avatars.githubusercontent.com/u/114952970?v=4?s=100" width="100px;" alt="Mohamed Ali Nor"/><br /><sub><b>Mohamed Ali Nor</b></sub></a><br /><a href="#promotion-IbnuAlii" title="Promotion">📣</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Suei43"><img src="https://avatars.githubusercontent.com/u/101181374?v=4?s=100" width="100px;" alt="Folarin Raphael "/><br /><sub><b>Folarin Raphael </b></sub></a><br /><a href="#a11y-Suei43" title="Accessibility">️️️️♿️</a> <a href="#question-Suei43" title="Answering Questions">💬</a> <a href="#blog-Suei43" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Suei43" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Suei43" title="Documentation">📖</a> <a href="#maintenance-Suei43" title="Maintenance">🚧</a> <a href="#platform-Suei43" title="Packaging/porting to new platform">📦</a> <a href="#plugin-Suei43" title="Plugin/utility libraries">🔌</a> <a href="#projectManagement-Suei43" title="Project Management">📆</a> <a href="#promotion-Suei43" title="Promotion">📣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3ASuei43" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Suei43" title="Tests">⚠️</a> <a href="#translation-Suei43" title="Translation">🌍</a> <a href="#userTesting-Suei43" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lutfiaomarr"><img src="https://avatars.githubusercontent.com/u/140343079?v=4?s=100" width="100px;" alt="lutfiaomarr"/><br /><sub><b>lutfiaomarr</b></sub></a><br /><a href="#a11y-lutfiaomarr" title="Accessibility">️️️️♿️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ali-Ahmed-Mohamed"><img src="https://avatars.githubusercontent.com/u/76924291?v=4?s=100" width="100px;" alt="Ali-Ahmed-Mohamed"/><br /><sub><b>Ali-Ahmed-Mohamed</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Ali-Ahmed-Mohamed" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/fab33150"><img src="https://avatars.githubusercontent.com/u/31627257?v=4?s=100" width="100px;" alt="Fabrice Innocent"/><br /><sub><b>Fabrice Innocent</b></sub></a><br /><a href="#blog-fab33150" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=fab33150" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Afab33150" title="Reviewed Pull Requests">👀</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/beckyrich"><img src="https://avatars.githubusercontent.com/u/63355222?v=4?s=100" width="100px;" alt="Becky Richardson"/><br /><sub><b>Becky Richardson</b></sub></a><br /><a href="#blog-beckyrich" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Abeckyrich" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=beckyrich" title="Code">💻</a> <a href="#content-beckyrich" title="Content">🖋</a> <a href="#design-beckyrich" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=beckyrich" title="Documentation">📖</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://www.chrisnowicki.io/"><img src="https://avatars.githubusercontent.com/u/102450568?v=4?s=100" width="100px;" alt="Chris Nowicki"/><br /><sub><b>Chris Nowicki</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=chris-nowicki" title="Code">💻</a> <a href="#blog-chris-nowicki" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=chris-nowicki" title="Documentation">📖</a> <a href="#tutorial-chris-nowicki" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Franklyn883"><img src="https://avatars.githubusercontent.com/u/67758035?v=4?s=100" width="100px;" alt="Frank Alimimian"/><br /><sub><b>Frank Alimimian</b></sub></a><br /><a href="#blog-Franklyn883" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Franklyn883" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Franklyn883" title="Documentation">📖</a> <a href="#research-Franklyn883" title="Research">🔬</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://danott.dev/"><img src="https://avatars.githubusercontent.com/u/360261?v=4?s=100" width="100px;" alt="Dan Ott"/><br /><sub><b>Dan Ott</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=danieltott" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/samgkigotho"><img src="https://avatars.githubusercontent.com/u/116047791?v=4?s=100" width="100px;" alt="Samgkigotho"/><br /><sub><b>Samgkigotho</b></sub></a><br /><a href="#blog-samgkigotho" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Asamgkigotho" title="Bug reports">🐛</a> <a href="#content-samgkigotho" title="Content">🖋</a> <a href="#data-samgkigotho" title="Data">🔣</a> <a href="#design-samgkigotho" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=samgkigotho" title="Documentation">📖</a> <a href="#example-samgkigotho" title="Examples">💡</a> <a href="#ideas-samgkigotho" title="Ideas, Planning, & Feedback">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ant-Shell"><img src="https://avatars.githubusercontent.com/u/100455148?v=4?s=100" width="100px;" alt="Anthony Shellman"/><br /><sub><b>Anthony Shellman</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Ant-Shell" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Ant-Shell" title="Documentation">📖</a> <a href="#research-Ant-Shell" title="Research">🔬</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/alanoteles"><img src="https://avatars.githubusercontent.com/u/1028089?v=4?s=100" width="100px;" alt="Alano Teles"/><br /><sub><b>Alano Teles</b></sub></a><br /><a href="#question-alanoteles" title="Answering Questions">💬</a> <a href="#blog-alanoteles" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=alanoteles" title="Code">💻</a> <a href="#content-alanoteles" title="Content">🖋</a> <a href="#data-alanoteles" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=alanoteles" title="Documentation">📖</a> <a href="#research-alanoteles" title="Research">🔬</a> <a href="#translation-alanoteles" title="Translation">🌍</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ht-l1"><img src="https://avatars.githubusercontent.com/u/106502799?v=4?s=100" width="100px;" alt="Hannah Lin"/><br /><sub><b>Hannah Lin</b></sub></a><br /><a href="#question-ht-l1" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Aht-l1" title="Bug reports">🐛</a> <a href="#business-ht-l1" title="Business development">💼</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ht-l1" title="Code">💻</a> <a href="#ideas-ht-l1" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-ht-l1" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-ht-l1" title="Maintenance">🚧</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://ethenportfolio.vercel.app/"><img src="https://avatars.githubusercontent.com/u/104235709?v=4?s=100" width="100px;" alt="Ethen Roth"/><br /><sub><b>Ethen Roth</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3AEthenThinkful" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=EthenThinkful" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=EthenThinkful" title="Documentation">📖</a> <a href="#ideas-EthenThinkful" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AEthenThinkful" title="Reviewed Pull Requests">👀</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tedashikode"><img src="https://avatars.githubusercontent.com/u/57563873?v=4?s=100" width="100px;" alt="koder_"/><br /><sub><b>koder_</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=tedashikode" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=tedashikode" title="Documentation">📖</a> <a href="#example-tedashikode" title="Examples">💡</a> <a href="#ideas-tedashikode" title="Ideas, Planning, & Feedback">🤔</a> <a href="#research-tedashikode" title="Research">🔬</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/code99-ash"><img src="https://avatars.githubusercontent.com/u/64657035?v=4?s=100" width="100px;" alt="Ikhlas"/><br /><sub><b>Ikhlas</b></sub></a><br /><a href="#audio-code99-ash" title="Audio">🔊</a> <a href="#blog-code99-ash" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Acode99-ash" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=code99-ash" title="Code">💻</a> <a href="#design-code99-ash" title="Design">🎨</a> <a href="#ideas-code99-ash" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Acode99-ash" title="Reviewed Pull Requests">👀</a> <a href="#security-code99-ash" title="Security">🛡️</a> <a href="#userTesting-code99-ash" title="User Testing">📓</a> <a href="#video-code99-ash" title="Videos">📹</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://linkfree.eddiehub.io/CBID2"><img src="https://avatars.githubusercontent.com/u/105683440?v=4?s=100" width="100px;" alt="Christine Belzie"/><br /><sub><b>Christine Belzie</b></sub></a><br /><a href="#a11y-CBID2" title="Accessibility">️️️️♿️</a> <a href="#blog-CBID2" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3ACBID2" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=CBID2" title="Code">💻</a> <a href="#content-CBID2" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=CBID2" title="Documentation">📖</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3ACBID2" title="Reviewed Pull Requests">👀</a> <a href="#tutorial-CBID2" title="Tutorials">✅</a> <a href="#example-CBID2" title="Examples">💡</a> <a href="#ideas-CBID2" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-CBID2" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-CBID2" title="Maintenance">🚧</a> <a href="#mentoring-CBID2" title="Mentoring">🧑‍🏫</a> <a href="#plugin-CBID2" title="Plugin/utility libraries">🔌</a> <a href="#projectManagement-CBID2" title="Project Management">📆</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3ACBID2" title="Reviewed Pull Requests">👀</a> <a href="#security-CBID2" title="Security">🛡️</a> <a href="#tool-CBID2" title="Tools">🔧</a> <a href="#translation-CBID2" title="Translation">🌍</a> <a href="#tutorial-CBID2" title="Tutorials">✅</a> <a href="#userTesting-CBID2" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/diegorramos84"><img src="https://avatars.githubusercontent.com/u/17050237?v=4?s=100" width="100px;" alt="Diego Ramos"/><br /><sub><b>Diego Ramos</b></sub></a><br /><a href="#a11y-diegorramos84" title="Accessibility">️️️️♿️</a> <a href="#blog-diegorramos84" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Adiegorramos84" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=diegorramos84" title="Code">💻</a> <a href="#content-diegorramos84" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=diegorramos84" title="Documentation">📖</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Adiegorramos84" title="Reviewed Pull Requests">👀</a> <a href="#tutorial-diegorramos84" title="Tutorials">✅</a> <a href="#example-diegorramos84" title="Examples">💡</a> <a href="#ideas-diegorramos84" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-diegorramos84" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-diegorramos84" title="Maintenance">🚧</a> <a href="#mentoring-diegorramos84" title="Mentoring">🧑‍🏫</a> <a href="#plugin-diegorramos84" title="Plugin/utility libraries">🔌</a> <a href="#projectManagement-diegorramos84" title="Project Management">📆</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Adiegorramos84" title="Reviewed Pull Requests">👀</a> <a href="#security-diegorramos84" title="Security">🛡️</a> <a href="#tool-diegorramos84" title="Tools">🔧</a> <a href="#translation-diegorramos84" title="Translation">🌍</a> <a href="#tutorial-diegorramos84" title="Tutorials">✅</a> <a href="#userTesting-diegorramos84" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/thititongumpun"><img src="https://avatars.githubusercontent.com/u/55313215?v=4?s=100" width="100px;" alt="thititongumpun"/><br /><sub><b>thititongumpun</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Athititongumpun" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=thititongumpun" title="Code">💻</a> <a href="#data-thititongumpun" title="Data">🔣</a> <a href="#design-thititongumpun" title="Design">🎨</a> <a href="#infra-thititongumpun" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/jayasuryard31"><img src="https://avatars.githubusercontent.com/u/92865629?v=4?s=100" width="100px;" alt="Jayasurya R D"/><br /><sub><b>Jayasurya R D</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=jayasuryard31" title="Code">💻</a> <a href="#data-jayasuryard31" title="Data">🔣</a> <a href="#ideas-jayasuryard31" title="Ideas, Planning, & Feedback">🤔</a> <a href="#design-jayasuryard31" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Ajayasuryard31" title="Reviewed Pull Requests">👀</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Obasoro"><img src="https://avatars.githubusercontent.com/u/29310552?v=4?s=100" width="100px;" alt="Obasoro"/><br /><sub><b>Obasoro</b></sub></a><br /><a href="#a11y-Obasoro" title="Accessibility">️️️️♿️</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3AObasoro" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Obasoro" title="Code">💻</a> <a href="#content-Obasoro" title="Content">🖋</a> <a href="#data-Obasoro" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Obasoro" title="Documentation">📖</a> <a href="#example-Obasoro" title="Examples">💡</a> <a href="#ideas-Obasoro" title="Ideas, Planning, & Feedback">🤔</a> <a href="#infra-Obasoro" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#mentoring-Obasoro" title="Mentoring">🧑‍🏫</a> <a href="#research-Obasoro" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AObasoro" title="Reviewed Pull Requests">👀</a> <a href="#security-Obasoro" title="Security">🛡️</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Obasoro" title="Tests">⚠️</a> <a href="#tool-Obasoro" title="Tools">🔧</a> <a href="#userTesting-Obasoro" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dxeon"><img src="https://avatars.githubusercontent.com/u/9787379?s=100" width="100px;" alt="Dmitry"/><br /><sub><b>Dmitry</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=dxeon" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://wasscodeur.me/"><img src="https://avatars.githubusercontent.com/u/100234404?v=4?s=100" width="100px;" alt="Wachiou BOURAÏMA"/><br /><sub><b>Wachiou BOURAÏMA</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=WassCodeur" title="Code">💻</a> <a href="#question-WassCodeur" title="Answering Questions">💬</a> <a href="#business-WassCodeur" title="Business development">💼</a> <a href="#content-WassCodeur" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=WassCodeur" title="Documentation">📖</a> <a href="#ideas-WassCodeur" title="Ideas, Planning, & Feedback">🤔</a> <a href="#promotion-WassCodeur" title="Promotion">📣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=WassCodeur" title="Tests">⚠️</a> <a href="#translation-WassCodeur" title="Translation">🌍</a> <a href="#tutorial-WassCodeur" title="Tutorials">✅</a> <a href="#userTesting-WassCodeur" title="User Testing">📓</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://david-001.github.io/website/"><img src="https://avatars.githubusercontent.com/u/9206557?v=4?s=100" width="100px;" alt="David Akim"/><br /><sub><b>David Akim</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=david-001" title="Code">💻</a> <a href="#content-david-001" title="Content">🖋</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Satoshi-Sh"><img src="https://avatars.githubusercontent.com/u/73622805?v=4?s=100" width="100px;" alt="Satoshi Sh."/><br /><sub><b>Satoshi Sh.</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Satoshi-Sh" title="Code">💻</a> <a href="#content-Satoshi-Sh" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Satoshi-Sh" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/geoffreylgv"><img src="https://avatars.githubusercontent.com/u/52314615?v=4?s=100" width="100px;" alt="Geoffrey Logovi"/><br /><sub><b>Geoffrey Logovi</b></sub></a><br /><a href="#design-geoffreylgv" title="Design">🎨</a> <a href="#translation-geoffreylgv" title="Translation">🌍</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=geoffreylgv" title="Documentation">📖</a> <a href="#content-geoffreylgv" title="Content">🖋</a> <a href="#tutorial-geoffreylgv" title="Tutorials">✅</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3Ageoffreylgv" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=geoffreylgv" title="Code">💻</a> <a href="#blog-geoffreylgv" title="Blogposts">📝</a> <a href="#video-geoffreylgv" title="Videos">📹</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Ageoffreylgv" title="Bug reports">🐛</a> <a href="#example-geoffreylgv" title="Examples">💡</a> <a href="#promotion-geoffreylgv" title="Promotion">📣</a> <a href="#projectManagement-geoffreylgv" title="Project Management">📆</a> <a href="#ideas-geoffreylgv" title="Ideas, Planning, & Feedback">🤔</a> <a href="#plugin-geoffreylgv" title="Plugin/utility libraries">🔌</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/goobric"><img src="https://avatars.githubusercontent.com/u/23141638?v=4?s=100" width="100px;" alt="Mikal"/><br /><sub><b>Mikal</b></sub></a><br /><a href="#a11y-goobric" title="Accessibility">️️️️♿️</a> <a href="#question-goobric" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=goobric" title="Code">💻</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=goobric" title="Documentation">📖</a> <a href="#ideas-goobric" title="Ideas, Planning, & Feedback">🤔</a> <a href="#mentoring-goobric" title="Mentoring">🧑‍🏫</a> <a href="#tutorial-goobric" title="Tutorials">✅</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://www.freecodecamp.org/news/author/tooba/"><img src="https://avatars.githubusercontent.com/u/52610124?v=4?s=100" width="100px;" alt="Tooba Jamal"/><br /><sub><b>Tooba Jamal</b></sub></a><br /><a href="#a11y-ToobaJamal" title="Accessibility">️️️️♿️</a> <a href="#question-ToobaJamal" title="Answering Questions">💬</a> <a href="#blog-ToobaJamal" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3AToobaJamal" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ToobaJamal" title="Code">💻</a> <a href="#content-ToobaJamal" title="Content">🖋</a> <a href="#data-ToobaJamal" title="Data">🔣</a> <a href="#design-ToobaJamal" title="Design">🎨</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ToobaJamal" title="Documentation">📖</a> <a href="#eventOrganizing-ToobaJamal" title="Event Organizing">📋</a> <a href="#example-ToobaJamal" title="Examples">💡</a> <a href="#ideas-ToobaJamal" title="Ideas, Planning, & Feedback">🤔</a> <a href="#maintenance-ToobaJamal" title="Maintenance">🚧</a> <a href="#mentoring-ToobaJamal" title="Mentoring">🧑‍🏫</a> <a href="#projectManagement-ToobaJamal" title="Project Management">📆</a> <a href="#promotion-ToobaJamal" title="Promotion">📣</a> <a href="#research-ToobaJamal" title="Research">🔬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AToobaJamal" title="Reviewed Pull Requests">👀</a> <a href="#talk-ToobaJamal" title="Talks">📢</a> <a href="#tool-ToobaJamal" title="Tools">🔧</a> <a href="#translation-ToobaJamal" title="Translation">🌍</a> <a href="#tutorial-ToobaJamal" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ZeeshanMukhtar1"><img src="https://avatars.githubusercontent.com/u/91063160?v=4?s=100" width="100px;" alt="Zeeshan Mukhtar"/><br /><sub><b>Zeeshan Mukhtar</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ZeeshanMukhtar1" title="Code">💻</a> <a href="#content-ZeeshanMukhtar1" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ZeeshanMukhtar1" title="Documentation">📖</a> <a href="#example-ZeeshanMukhtar1" title="Examples">💡</a> <a href="#ideas-ZeeshanMukhtar1" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AZeeshanMukhtar1" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=ZeeshanMukhtar1" title="Tests">⚠️</a> <a href="#translation-ZeeshanMukhtar1" title="Translation">🌍</a> <a href="#tutorial-ZeeshanMukhtar1" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/codewithjazzy"><img src="https://avatars.githubusercontent.com/u/105261487?v=4?s=100" width="100px;" alt="Jasmine"/><br /><sub><b>Jasmine</b></sub></a><br /><a href="#tutorial-codewithjazzy" title="Tutorials">✅</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ajiboso-Adeola"><img src="https://avatars.githubusercontent.com/u/79532937?v=4?s=100" width="100px;" alt="Ajiboso Adeola"/><br /><sub><b>Ajiboso Adeola</b></sub></a><br /><a href="#question-Ajiboso-Adeola" title="Answering Questions">💬</a> <a href="#blog-Ajiboso-Adeola" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Ajiboso-Adeola" title="Code">💻</a> <a href="#content-Ajiboso-Adeola" title="Content">🖋</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Ajiboso-Adeola" title="Documentation">📖</a> <a href="#a11y-Ajiboso-Adeola" title="Accessibility">️️️️♿️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JesseRWeigel"><img src="https://avatars.githubusercontent.com/u/11077930?v=4?s=100" width="100px;" alt="Jesse Weigel"/><br /><sub><b>Jesse Weigel</b></sub></a><br /><a href="#question-JesseRWeigel" title="Answering Questions">💬</a> <a href="#blog-JesseRWeigel" title="Blogposts">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=JesseRWeigel" title="Code">💻</a> <a href="#a11y-JesseRWeigel" title="Accessibility">️️️️♿️</a> <a href="#video-JesseRWeigel" title="Videos">📹</a> <a href="https://github.com/TejasQ/opensauced-guestbook/pulls?q=is%3Apr+reviewed-by%3AJesseRWeigel" title="Reviewed Pull Requests">👀</a></td>
        <td align="center" valign="top" width="14.28%"><a href="https://github.com/VirginieLemaire"><img src="https://avatars.githubusercontent.com/u/82816247?v=4?s=100" width="100px;" alt="Virginie"/><br /><sub><b>Virginie</b></sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=VirginieLemaire" title="Code">💻</a> <a href="#data-VirginieLemaire" title="Data">🔣</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=VirginieLemaire" title="Documentation">📖</a> <a href="#ideas-VirginieLemaire" title="Ideas, Planning, & Feedback">🤔</a> <a href="#translation-VirginieLemaire" title="Translation">🌍</a></td>
    </tr>
<tr>    
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/vaibhavharsoda"><img src="https://avatars.githubusercontent.com/u/66860032?v=4?s=100" width="100px;" alt="Vaibhav Patel"/><br /><sub><b>Vaibhav Patel</b></sub></a><br /><a href="#question-vaibhavharsoda" title="Answering Questions">💬</a> <a href="https://github.com/TejasQ/opensauced-guestbook/issues?q=author%3Avaibhavharsoda" title="Bug reports">🐛</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=vaibhavharsoda" title="Code">💻</a> <a href="#design-vaibhavharsoda" title="Design">🎨</a> <a href="#ideas-vaibhavharsoda" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=vaibhavharsoda" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Lymah123"><img src="https://avatars.githubusercontent.com/u/109049037?v=4" width="100px;" alt="Harlimat Odunola"/><br /><sub><b>Harlimat Odunola</b>
      </sub></a><br /><a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Lymah123" title="Code">💻</a> 
        <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Lymah123" title="Blog">📝</a> <a href="https://github.com/TejasQ/opensauced-guestbook/commits?author=Lymah123" title="Documentation">📖</a> <a href="#answerLymah123" title="Answering Questions">💬</a>  <a href="#example-Lymah123" title="Example">📋</a>
  <a href="#translation-Lymah123" title="Translation">🌍</a> <a href="#content-Lymah123" title="Content">📦</a> <a href="#ideas-Lymah123" title="Ideas">💡</a> <a href="#review-Lymah123" title="Review">🔍</a> <a href="#test-Lymah123" title="Test">🧪</a> <a href="#tutorial-Lymah123" title="Tutorial">📚</a> <a href="#accessibility-Lymah123" title="Accessibility">️️♿</td> 
  
      </tr>  
  </tbody>
  <tfoot>
    <tr>
      <td align="center" size="13px" colspan="7">
        <img src="https://raw.githubusercontent.com/all-contributors/all-contributors-cli/1b8533af435da9854653492b1327a23a4dbd0a10/assets/logo-small.svg">
          <a href="https://all-contributors.js.org/docs/en/bot/usage">Add your contributions</a>
        </img>
      </td>
    </tr>
  </tfoot>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!
