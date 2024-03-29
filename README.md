# Hosting Your Resume via Github Pages

## Purpose
The purpose of this document is to describe the practical steps for hosting and formatting resume in markdown and relate them to general principles of current Technical Writing, as explained in Modern Technical Writing by Andrew Etter.

## Prerequisites
* GitHub Account: You will need a GitHub account to create your project and host your resume online as a static website. 
  * Explore GitHub here: [*What is GitHub and what does it offer?*](https://blog.hubspot.com/website/what-is-github-used-for)
  * Create a free account: [GitHub!](https://github.com)
* [Resume](index.md) - my resume formatted in Markdown. Also check [More Resources](#more-resources) for links to tutorials, free online editors, syntax documentation and more!

## Instructions
### 1. **Setting up your GitHub Repository**
* ***Concept of Etter's Book***: GitHub leverage's Git's version control system. What this means is that GitHub provides us a platform where we can manage both code and documentation in one place and also keep a track of all the changes we make. As Andrew Etter mentions in their book, using a version control system allows for collaboration among a team, and provides a common platform for team members to use. Following this, using GitHub will be a great tool for managing your online portfolio.
* ***Steps***:
  1. Sign in to your github account [here](https://github.com/login).
  2. Navigate to your dashboard and click on **New** button at the top left to create a new repository.
  3. Name your repository `[YourGitHubUsername].github.io`. This format ensures compatibility with the default settings of GitHub Pages as well as helps create a consistent URL for your website.
  4. Set the repository to **Public** to allow potential employers to view your static website.
  5. Check the **Add a README file** option to create a default README file. A README serves as an introduction to a repository and is visible on the repository home page, similar to one you are currently reading. 
### 2. **Formatting your Resume**
* ***Concept of Etter's Book***: Markdown is a simple and lighweight language with limited syntax and format. As mentioned in Etter's Book, using a straightforward language like Markdown makes writing the documentation more intuitive and the simple format allows for readers to focus more on content than the formatting. Following this concept, we will be hosting our resume via a Markdown formatted file.
* ***Steps***:
  1. Create a new file in your repository using the + button on top right and save it as **index.md**. This is *crucial* as GitHub Pages, by default, renders the static website content based on the index file. By saving your resume as index.md, it will allow GitHub Pages to display the content as the main page on the website.
  2. Format your resume content either directly in GitHub or by using a [Markdown editor](#more-resources).
  3. Input your resume content formatted using Markdown syntax in this file if applicable and save your changes using the green "Commit changes..." button on top right.
### 3. **Adding a Theme**
* ***Concept of Etter's Book***: GitHub Pages supports a list of Jekyll themes which allows users to create a cohesive static website. As Etter mentions in their book, it is vital to present all technical documentation in a visually appealing and consistent way. Applying [Jekyll Themes](#more-resources) allows us to do the same in simple steps. 
* ***Steps***:
  1. Create a new file named **_config.yml** in your repository.
  2. Add the following code to your config file: `theme: jekyll-theme-[Name of Theme]`. Refer to my [_config.yml file](_config.yml) for an example.
  3. *Optional*: You can also add other attributes like title, description and more to your website by adding `title: [page title]` or `description: [page description]` etc. to your config file. 
### 4. **Configuring static website**
* ***Concept of Etter's Book***: In Etter's book, they mention the importance of accessibility and straightforward depolyment of technical documentation. Following their model, we will host our resume on GitHub Pages: a built in feature of GitHub that allows us to generate static websites. By doing so, we ensure a few key things: consistent accessibility of our online resume as well as effortless editing and deployment of all applicable files.
* ***Steps***:
  1. Ensure all files are set up and committed properly.
  2. Navigate to your repository settings by clicking on the "Settings" tab on top. Go to "Pages" from the menu on the left.
  3. Select "Deploy from a branch" under Source. Additionally, select the "main" branch and "/ root" as the directory. This ensures that GitHub Pages will find the index file in the *root* directory of the *main* branch.
  4. Your static website is ready to viewed on a web browser at `https://[YourGitHubUsername].github.io`!
 
### Resume Demo via Animated Gif
![gif](https://github.com/simkaurd/simkaurd.github.io/blob/main/assets/resume.gif)


## More Resources
* [What is GitHub](https://blog.hubspot.com/website/what-is-github-used-for): an amazing blog that explains and introduces GitHub for beginners.
* [Tutorial](https://www.markdowntutorial.com/): practice Markdown for free!
* [StackEdit](https://stackedit.io): free online Markdown editor.
* [Syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax): basic Markdown syntax documentation by GitHub.
* [Static Website](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site): official GitHub documentation for hosting a static website via Github Pages.
* [GitHub supported Themes](https://pages.github.com/themes/): list of jekyll themes supported natively by GitHub.

## Acknowledgements
I would like to express my gratitude to Andrew Etter for their insight on Technical Writing via their book, Modern Technical Writing. Additionally, I appreciate my group members Vishal Singh Heer and Hridai Mehta for their valuable input and critique which helped polish this document. At last, I would like to acknowledge our professor, Stewart Wilcox for their aid in making this project possible!

## FAQs
1. Why is markdown better than a word processor?
* Markdown is a plain text file with limited syntax and features. While word processors offer high utility, Markdown offers simplicity and versatility which makes it an ideal choice for technical writing. Additionally, GitHub Pages features easy rendering of Markdown to HTML which allows us to create static websites without the need for advanced web development skills.

2. Why is my resume not showing on the static website?
* Please ensure all of these conditions are met for seemless rendering of your static website.
  * You *must* have your resume saved as "index.md" as GitHub pages picks up file named "index" as their base for the website and renders it into HTML.
  * You *must* have your "index.md" file in the root directory of your repository.
  * You *must* have your GitHub Pages configured properly - i.e. to build from root directory in the main branch.
  * You *must* ensure GitHub has finished building all changes. This will ensure you see the latest changes on your static website. 
