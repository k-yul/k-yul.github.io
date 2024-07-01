
# Development Instructions

This website uses https://gohugo.io/.

## Running the hugo server locally
In the terminal, run `hugo serve` to run the local server. It will automatically reload on changes to the content.

## Pushing (publishing) the changes to GitHub
In the terminal:
1. Stage the current changes `git add .` (this means add everything in the current directory)
2. Commit the current changes `git commit -m "some message describing your change"`
3. Push the changes to GitHub `git push`

After you push to GitHub, go to [Deployments](https://github.com/k-yul/k-yul.github.io/deployments) and monitor the status until it's a green checkmark. 

## Getting updates from the repository

If someone else pushes changes to the repository, `git pull` to get those changes to your local copy.

## Layout

* .github/workflows: Just has a configuration file to publish the website.
* archetypes: You can ignore this one.
* content/projects: This is where the content markdown files go. Each file is for a different post (project).
* layouts: This folder overrides the templates provided in the theme we're using. If there's a file here, it's because we wanted to change something in the default template. You can compare the stuff in here to the defaults in themes/hugo-profile/layouts
* public: Ignore this, when you run hugo serve it generates the actual html, css, js files for the static website.
* static: Make edits to the default css by editing the files in static/css. To add images add image files to static/images, then include them in the project files in contents/projects/*.md.
* hugo.yaml: This is a top-level configuration file. You can edit the text on the landing page, colors, enable/disable menus, etc. from here. 