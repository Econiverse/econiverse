---
weight: 20
title: How to Edit Locally
---

To make major edits to the website, such as adding pages or reorganizing the menu, it is highly recommended to edit the site locally, preview the edits, and then merge them into the main branch with GitHub. Here are the steps to do that:

{{< toc >}}

1. **Create a GitHub Account and Setup SSH**
   
   - Follow the instructions [here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh) to create a GitHub account and set up SSH.

2. **Clone the Repo**
   
   - Clone the repository to create a local copy that you can modify and test before committing it to the main project. You can find instructions [here](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository-from-github/cloning-a-repository).

3. **Install Hugo**
   
   - This site is built using Hugo, so make sure you have it installed locally to build the site. Refer to the installation instructions [here](https://gohugo.io/getting-started/installing/).

4. **Run the Site Locally**
   
   - Now that you have the entire site downloaded locally and Hugo installed, let's test it! Open your command line, navigate to the location where you cloned the *econiverse* repository, and run `hugo server -D`. This will start a local server, and you can view the website by opening *localhost:1313* in your browser.

5. **Download Visual Studio Code and Edit the Site**
   
   - Download and install Visual Studio Code from [here](https://code.visualstudio.com/). If you already have a preferred text editor and GitHub manager, feel free to skip this step. The following instructions will reference Visual Studio Code.
   - Open Visual Studio Code and add the *econiverse* folder to your workspace by navigating to *File -> Add Folder to Workspace* and selecting the cloned folder.
   
6. **Site Organization - Pages, Menu, and HTML**
   
   - **Pages:** The contents of each page can be found in the corresponding *_index.md* file within each folder. When creating a new page, make sure to create a new folder and a new *_index.md* file. You can explore the available features and formatting options in this submodule by referring to the [Geekdocs Features Documentation](https://geekdocs.de/features/code-blocks/).
   - **Menu:** The menu is the navigation list on the left side of the website. You can find the contents and organization of the menu in the *data -> menu -> main.yml* file. For more information, refer to the [Geekdocs Menu Documentation](https://geekdocs.de/usage/menus/). This site uses a bundle menu.
   - **HTML:** Adding HTML that is outside the scope of Hugo and this submodule is not recommended but sometimes unavoidable, such as adding videos. To add custom HTML, navigate to the *layouts -> shortcodes* folder and create a file that ends with *.html*, like *mycode.html*. Insert your HTML code in this file. You can then use this custom code on any page by using `{{</* mycode */>}}`. For example, to insert a .mp4 video, you can use the HTML shortcode that has already been created. Store the video in the *static -> videos* folder and insert it on any page using `{{</* addmp4vid myvideofile */>}}`.

7. **Commit and Push**
   
   - Once you've made your edits and previewed them locally, it's time to integrate them into the live website. In Visual Studio Code, use the Source Control tab on the left-hand side. Click the "+" icon to stage all changes, write a commit message, and click the checkmark icon to commit. Then, click the ellipsis icon (...) and select "Push" to push the changes to the remote repository.

That's it! Following these steps will enable you to make and preview edits locally before merging them into the live website.
