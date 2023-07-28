# Wordpress to Docusaurus

If you're used to writing and publishing posts in Wordpress then Docusaurus is a bit different. The main things to get used to are

* Write in markdown - instead of doing layout and formatting using a GUI, you'll add annotations to your text to specify things like italics, bold, lists, tables, and also for links and images.
* Version control your work with git - git is complicated, but it makes it easy to keep track different versions of your work. No more `draft_2_final_4.docx` files.

We'll demo how to add an article using GitHub.com. You might prefer to use your own editor like VSCode locally and work on a local copy of the repository, but you should be able to adapt the below to your workflow in that case.

## Creating a new file 

The Docusuarus content is all in a subfolder called `docs`, which mirrors the structure of the site itself (one subfolder per top-level section).

![screenshot 2023-07-28 at 10 35 24@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/eaf69f2c-a20e-4856-b5a3-89bf7392b074)

To create a new file, use the "add file" button

![screenshot 2023-07-28 at 10 36 37@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/e8d73590-703b-4ae4-8cb6-6becb6536e01)

Give the name a `.md` extension so that GitHub can preview the markdown content. In this example, we create a new folder too by adding the new folder name with `/` in the file name.

https://i.ritzastatic.com/images/3e8bcb45da5f427d876ebb52053d79f7/add-file.gif

Add the title and sidebar position as yaml metadata at the top of the file.

![screenshot 2023-07-28 at 10 41 57@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/481b1be1-4f57-43d3-9a1c-a0325f7a1c53)

Add any other markdown content below (do not repeat the title as this will be taken from the metadata)

Commit your work as often as you want (equivalent to saving the file). On the first commit, choose to create a new branch so you can keep working on a separate copy of the docs before merging your work into main.

![screenshot 2023-07-28 at 10 43 03@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/de6d25dd-f167-4746-88c4-ee5e2f4cd523)

Create a pull request into main

![screenshot 2023-07-28 at 10 44 41@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/970acdc2-fa7b-4aa6-a571-fc8b2fe9b309)


## Adding images

On the same branch, you can upload images that you need to reference in the post.

![screenshot 2023-07-28 at 10 47 01@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/e7ebb037-a8a6-403c-a663-82cf274e30be)

Upload your files and commit them

<img width="1311" alt="screenshot 2023-07-28 at 10 49 37@2x" src="https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/3e81293b-b06d-45a6-895c-318b7aca8a3b">

In your markdown file, you can now reference the images using `/assets/images/<subfolder>/imagename.png`

![screenshot 2023-07-28 at 11 32 58@2x](https://github.com/ritza-co/wordpress-to-docusaurus/assets/2641205/27733176-e18f-4951-af59-1e7b019c5398)

Note that images will not show in the GitHub preview as they are actually in a `static` folder that is treated differently by Docusaurus. You will need to run Docusuarus locally to properly preview the images as you write new content.
