# Hosting a Resume on Github Pages

## Table of Contents
* [Purpose](##Purpose)
* [Prerequisites](##Prerequisites)
* [Instructions](##Instructions)
* [More Resources](##More-Resources)
* [Author and Acknowledgements](##Authors-and-Acknolwedgements)
* [FAQs](#FAQs)

## Purpose 
There are 2 primary purposes of this document:
1. Explain how to host a resume on Github Pages
2. Relate the practical steps of hosting a resume to the general principles of technical writing described in Andrew Etter's book *Modern Tehnical Writing*

## Prerequisites

Before following this guide, the following prerequisites are required:
- An account on [Github.com](https://github.com/)
- A resume formatted in Markdown

## Instructions 

### Creating a Repository
1. Select the "+" icon in the upper right-hand corner of any page and click "New Repository"
2. Enter `username.github.io` as the repository name, replacing `username` with your own Github username
3. Click "Create Repository"

This step relates to Etter's principle of using a distributed version control system. Distributed version control systems like GitHub are useful because they allow multiple contributors to work on the same document concurrently. Since each contibutor has a their own copy of the files, they can also work offline if needed.
### Uploading your resume

1. Rename your Markdown resume file to `index.md`. This step will allow Github to recognize which file should be used to generate your website
1. Choose "start by uploading a file" under the Quick Start menu on your repository page 
2. Upload your Markdown resume file by selecting "Choose your files" or by dragging the file onto the upload window
3. Click "Commit Changes"

This step relates to Etter's principle of using a lightweight markup language. Lightweight markup languages like Markdown have small file sizes which make them ideal for hosting on version control systems. They are also easy to learn and compatible with many software platforms.

### Hosting your resume with GitHub Pages
1. Navigate to the Settings page located in the top menu bar of your repository
2. Click Pages (located in the left-hand menu under Code and Automation)
3. Under Build and Deployment, make sure the following options are selected:
    - Source should be set to "Deploy from a branch"
    - Branch should be set to "main" with folder "root"
4. Navigate to `https://username.github.io/` to view your generated website. Note that the process of deploying your website may take a few minutes to complete

This step relates to Etter's principle of building a website. Unlike PDFs or other document types, websites can be easily updated for new versions of software or to fix any inaccuracies.

### Adding a Jekyll Theme
1. Choose a theme you would like to use for your resume. A list of supported themes can be found [here](https://pages.github.com/themes/)
1. Click "Add File" and select Create new file
2. Name the new file `_config.yml` by entering the filename at the top of the file editor window
3. Add the following text to the config file theme: `jekyll-theme-THEME-NAME`  (replacing `THEME-NAME` with the theme of your choice from the list of supported themes)
4. Click "Commit changes..." in the top right corner. This will open a Commit changes pop-up window
5. Cick "Commit changes" in the pop-up window. All other options can be left as default
6. Navigate to https://username.github.io/ to view your generated website. Note that the process of deploying your website may take a few minutes to complete

This step relates to Etter's principle of making a static website. Static sites are simple, lightweight, and secure. Static site generators like Jekyll take in Markdown files and automatically generate a nicely formatted website, allowing the writer to focus on the actual content.

Once completed, your resume will look something like this:

![](resume.gif)

## More Resources

- [Markdown Guide](https://www.markdownguide.org/)
- [*Modern Technical Writing*](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) by Andrew Etter
- [Github Pages Documentation](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)

## Authors and Acknowledgements

This guide was written by Jonathan Placatka. Contact me at placatkj@myumanitoba.ca

Special thanks to:
- The [authors](https://github.com/pages-themes/hacker/graphs/contributors) of the Hacker theme for Github Pages 
- Heejeong Kim and Kevin Tsang for helping review and edit this guide.

## FAQs  

- **Why is Markdown better than a Word Processor?**
  - Markdown is lightweight, making it a good choice for files that are stored on version control systems and continuously updated
  - Markdown is widely used and easy to integrate with a variety of operating systems and software platforms.

- **Why is my resume not showing up?** Common probems include:

  - Incorrect filename - double check that your resume file is correctly named `index.md`
  - Build/deploy process not finished - it can take a few minutes for your resume to appear. You can check the deploy status on your repository code page. An orange circle indicates that the build is in progress, while a green check indicates that the build is complete.






























