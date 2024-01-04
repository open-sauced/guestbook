# Contributing to OpenSauced Guestbook

Contributions are always welcome, no matter how large or small. Before you begin, please read our [Code of Conduct](https://docs.opensauced.pizza/contributing/code-of-conduct/) and follow the directions below:

## Recommended Communication Style

1. Always leave screenshots for visual changes.
2. Always leave a detailed description in the Pull Request. Leave nothing ambiguous for the reviewer(s).
3. Always review your code first. Be sure to run the project locally and test it before asking for a review.
4. Always communicate in the GitHub repository. Whether it is in the issue or the pull request, keeping the lines of communication open and visible to everyone on the team helps everyone around you.

## Issues

If you wish to work on an open issue, please comment on the issue with `.take` and it will be assigned to you. If an issue is not assigned, it is assumed to be open for anyone to work on. Please assign yourself to an issue before beginning work on it to avoid conflicts.

If you are contributing to the project for the first time, please consider checking the [bug](https://github.com/open-sauced/intro/issues?q=is%3Aissue+is%3Aopen+label%3A%22%F0%9F%90%9B+bug%22) or [good first issue](https://github.com/open-sauced/intro/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) labels.

In case you get stuck, please feel free to ask for help in the [Discord](https://discord.com/invite/U2peSNf23P) server or GitHub Discussions.

## Setup the Project Locally

1. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the [guestbook repository](https://github.com/open-sauced/guestbook) you are working on to your own GitHub account.
2. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) the forked repository to your local machine.

   ```bash
   git clone https://github.com/<your-username>/guestbook.git
   ```

3. cd into the repository and open the project in your code editor.

   ```bash
   cd guestbook
   ```

4. Run the course locally. See [Running the Project Locally](#running-the-project-locally) for more information.

### Running the Project Locally

To contribute effectively to the OpenSauced project, it's essential to run the project locally to see your changes in action and test them thoroughly. We recommend two methods for running the project on your local machine: using the Docsify CLI or leveraging Visual Studio Code's Go Live feature.

#### Method 1: Using the Docsify CLI

1. **Install Node.js**: You can download it from the official Node.js [website](https://nodejs.org/.)
2. **Install Docsify Globally**: Open your command-line interface (CLI) and run the following command to install Docsify globally.

   ```bash
   npm install -g docsify-cli
   ```

3. Run the project locally:

   ```bash
   docsify serve
   ```

   This command will start a local development server, and you can access the documentation in your web browser at `http://localhost:3000`

4. Make and Test Changes: With the local server running, you can make changes to the documentation files and immediately see the results in your browser. Test your changes thoroughly.
5. Stop the Server: When you're done testing or making changes, you can stop the local server by pressing `Ctrl + C` in the CLI.

#### Method 2: Using Visual Studio Code (VS Code) Go Live Feature

Once you have cloned the repository to your local machine, you can use VS Code's Go Live feature to run the project locally. This feature allows you to launch a local development server and preview your changes in real time in your browser.

1. **Install Visual Studio Code**: Download and install [Visual Studio Code](https://code.visualstudio.com/).
2. **Open the Project in VS Code**: Launch VS Code and open the project folder by selecting "File" > "Open Folder" and choosing the project directory.
3. **Install the Live Server Extension**: In VS Code, navigate to the Extensions view (you can press `Ctrl + Shift + X`) and search for "Live Server. Install the "Live Server" extension by Ritwick Dey.

4. **Launch the Live Server**: In the opened HTML file, you should see a "Go Live" button in the bottom-right corner of the VS Code window. Click this button to launch the live server.

This will open your documentation in a new browser tab at a local address (typically `http://127.0.0.1:5500`).

6. **Make and Test Changes**: With the Live Server running, you can make changes to the documentation files using VS Code, and the changes will be automatically reflected in your browser. Test your changes thoroughly.

7. **Stop the Live Server**: When you're done testing or making changes, you can stop the Live Server by clicking the "Exit" button in the VS Code status bar.

## Adding a New Section to the Documentation

Welcome to the documentation contribution guide. In this guide, you will learn how to add a new section to our project's documentation. We have specific conventions for numbering sections to maintain a consistent structure.

## Using Markdown for Documentation

Markdown is a lightweight and easy-to-use markup language that allows you to format text in a readable and visually appealing way. When contributing to the documentation in this repository, it's important to use Markdown to structure and format your content effectively.

### Markdown Basics

Here are some common Markdown elements you can use:

#### 1. Headings

Use the hash (`#`) symbol to create headings (titles and subtitles). There are six levels of section headings, and the number of symbols indicates the heading level.

```markdown
# Heading 1

## Heading 2
```

#### 2. Text Formatting

- Make text bold by enclosing it with double asterisks (`**`).
- Make text italic by enclosing it with single underscores (`_`).
- Create inline code by wrapping text with backticks (`` ` ``).

```markdown
**This is a bold text.**

_This is an italic text._

This is an `inline code`.
```

#### 3. Lists

- Create ordered lists using numbers followed by a period (`1.`, `2.`, etc.).
- Create unordered lists using hyphens (`-`).

```markdown
1.  Item 1
2.  Item 2

- Unordered Item 1
- Unordered Item 2
```

#### 4. Links

Create links using square brackets (`[]`) for the link text and parentheses (`()`) for the URL.

```markdown
[Intro to Open Source with OpenSauced](https://intro.opensauced.pizza/#/)
```

#### 5. Images

Embed images using an exclamation mark (`!`), followed by square brackets (`[]`) for the alt text, and parentheses (`()`) for the image URL.

```markdown
![OpenSauced Highlights](https://github.com/open-sauced/intro/blob/main/images/opensauced-highlights.png)
```

#### 6. Blockquotes

Create blockquotes using the greater-than symbol (`>`).

```markdown
> This is a blockquote.
```

#### 7. Code Blocks

Create code blocks using triple backticks (` ``` `) for fenced code blocks and specify a language next to the backticks before the fenced code block to highlight the syntax.

````
```bash
git pull
```
````

### Markdown Tips

- Preview your Markdown locally to ensure proper formatting before submitting your contribution.
- Keep your Markdown content organized, and use headings to structure the sections.
- Use code blocks to highlight code snippets or configuration examples.
- Check out the official [Markdown Guide](https://www.markdownguide.org/basic-syntax/) website for more information about using Markdown.

## Adding Translations to Documentation

Adding translations to our project's documentation helps make it more accessible to a wider audience. If you're interested in contributing translations for our documentation, check out the below section.

### Steps to Add Translations

**1. Identify Target Languages:**

- Determine which languages you want to add translations for. Make sure these languages are relevant to the project's user base.

**2. Create Translation Files:**

- Inside the documentation directory, create a new subdirectory for each language you plan to support. Use language codes (e.g., "en" for English, "fr" for French) as directory names.

```bash
- docs/
  - en/         (English)
  - fr/         (French)
  - es/         (Spanish)
```

**3. Translate Content:**

- For each language directory, create translated versions of the documentation files. Typically, you will translate Markdown files, but consider other formats as needed.
- Maintain the same file structure and filenames as in the original documentation, but with translated content.

**4 Update Links:**

- In the translated files, ensure that any internal links (e.g., links to other sections or pages within the documentation) are updated to point to the corresponding translated content.

**5. Add Language Selector:**

- Consider adding a language selector to the documentation, allowing users to switch between different language versions. You can do this by modifying the navigation or header of your documentation.

**6. Testing and Validation:**

- Test the translated documentation to ensure accuracy and readability. Make sure that all links work correctly and that the content is culturally appropriate.

**7. Submit Contributions:**

- If you haven't already, submit your translations as a pull request. Ensure that you provide clear information about the languages you've translated and any specific details related to your contributions.

**8. Collaborate and Review:**

- Collaborate with other contributors and reviewers to ensure the quality of translations. Be open to feedback and suggestions for improvement.

### Best Practices for Translations

- Maintain consistency in terminology and style throughout the translated documentation.
- Work with another contributor who speaks the language you're translating to.
- It helps to mention specific tools so that developers who want to translate documentation can see how it's done.
- Keep translations up to date with changes in the original documentation.
