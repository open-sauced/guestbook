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

7. Add and commit your changes by running this command:

   ```bash
   git commit -am "Your message"
   ```

   Change `"Your message"` to your own message. For example, `"Add Alice to the guestbook"`.

   **You can skip this step (7) if you use the CLI tool to add yourself to the guestbook**.

8. Run `git log` to check if you have committed your changes. Press `Q` to close the log.

   If you add yourself using the CLI tool, it automatically adds and commits your changes. So you will see this automated commit message:

   ```bash
   docs: add @your_username as a contributor
   ```

9. Push the commit to your forked repository with this command:

   ```bash
   git push -u origin branch-name
   ```

10. Go to your forked repository on GitHub and [create a pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).

## Congratulations on your first contribution! 🎉

You can add this contribution to your [OpenSauced](https://opensauced.pizza) resume and profile as [outlined in the course](https://github.com/open-sauced/intro/blob/main/05-how-to-contribute-to-open-source.md)!

---

## 🤝 Contributing

All contributors are required to abide by our [Code of Conduct](https://github.com/open-sauced/.github/blob/main/CODE_OF_CONDUCT.md). Please follow the Readme directions for contributing.

## Contributors

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
