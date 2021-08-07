To make major edits to the website, such as adding pages or reorganizing the menu
it is highly recommended to edit the site locally, preview the edits, and then
merge it into the main branch with GitHub. Here are the steps to do that!

{{< toc >}}


## Create a GitHub Account and Setup SSH

Instructions for how to do this can be found [here](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh).

## Clone the Repo

Cloning the repository creates a local copy that you can modify and test before
committing it to the main project. Instructions can be found [here](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository-from-github/cloning-a-repository).

## Install Hugo

This site is built using hugo so you must have it locally in order to build the
site. Instructions for how to install it can be found [here](https://gohugo.io/getting-started/installing/).

## Run the Site Locally

At this point, you should have then entire site downloaded locally and a way to
run it, so, let's test it! Using the command line, navigate to the location where
you cloned *econiverse*. Once there, run `hugo server -D`. You should be able
to open the website by navigating to *localhost:1313* in your browser.

## Download Atom

This step is recommended. If you already have a text editor and GitHub manager,
feel free to skip this step. The rest of this guide will be referencing Atom.

Download Atom [here](https://atom.io/).

## Edit the Site!

At this point, you have everything you need to make edits and view them locally.
Open Atom, navigate to *File -> Add Project Folder*, and then add *econiverse*
folder that you previously cloned.  

## Site Organization

### Menu
The menu is the navigation list on the left side of the website. The contents and
organization of the menu can be found in the *data -> menu -> main.yml* file and
more information can be found [here](https://geekdocs.de/usage/menus/). This site
uses a bundle menu.

### Pages

Contents of each page can be found in the corresponding *_index.md* file, in the
within each folder. When a new page is created, a new folder and a new *_index.md*
file must be created. A list of features that are provided in this submodule and
can be used in building this website, such as code blocks, buttons, columns, hints,
equations, etc., can be found [here](https://geekdocs.de/features/code-blocks/).

## Commit and Push

Once your edits are made, and you have previewed them to ensure the site functions
correctly, it is time to integrate them to the live website. This can be done by
navigating to the Git tab in the bottom right of Atom. Once there, click
Stage All, write a short message, and click Commit to main. Then click the
Push button that appears in the bottom right. That's it!

## Adding html

Adding html that is outside the scope of hugo and this submodule is not recommended
but sometimes unavoidable, such as adding videos. To do this, navigate to the
*layouts -> shortcodes* folder. Create a file that ends with *.html*, such as
*mycode.html* and insert your html code in here. This code can then be used in
any page by using `{{</* mycode */>}}`.

To insert a .mp4 video, for example, you can use the html shortcode that has
already been created. Store the video in the *static -> videos* folder, and
insert the video in any page using `{{</* addmp4vid myvideofile */>}}`.
