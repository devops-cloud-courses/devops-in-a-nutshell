# Reveal Presentation Template

This a template project allowing you to start creating presentation content quicker with preconfigured Reveal.js project. 

## Setup
* Go to [repo main page](https://github.com/arthurmauvezin/reveal-presentation-template)
* Click on `Use this template` button 
* On creation page, choose your **org** or **profile** and fill **repository name** and click on `Create repository from template` button
* On your newly project landing page, go to **Settings** and enable **GitHub Pages**
* Then edit Description field with folowing parameter
  * Description: View live presentation here:
  * Website: Url to access live version of your course (this URL can be found in Settings >> Github Pages)
> For example, this repository description should contains URL https://arthurmauvezin.github.io/reveal-presentation-template
* In you new repository, replace all replace strings with your project values
```bash
sed -i 's/REPLACE_TITLE/<presentation_title>/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_SUBTITLE/<presentation_subtitle>/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_GITHUB_ACCOUNT/<github_account>/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_GITHUB_REPO_NAME/<github_repo_name>/g' index.html Readme.md slides/introduction.md
# Examples
sed -i 's/REPLACE_TITLE/DevOps/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_SUBTITLE/In a nutshell/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_GITHUB_ACCOUNT/arthurmauvezin/g' index.html Readme.md slides/introduction.md
sed -i 's/REPLACE_GITHUB_REPO_NAME/devops-in-a-nutshell/g' index.html Readme.md slides/introduction.md
```
* Commit and push your changes
```bash
git add index.html Readme.md slides/introduction.md
git commit -m "Initialize course content"
git push
```
* Delete this line and all lines above to get a clean Readme.md and commit and push your repository

# REPLACE_TITLE course

This repo contains a reveal.js presentation about REPLACE_TITLE.
To visualize this presentation, go here: https://REPLACE_GITHUB_ACCOUNT.github.io/REPLACE_GITHUB_REPO_NAME
You can also clone this repo and expose static pages through your favorite web server.

> This course is open source. You can use it freely.

## Table of content

* Introduction
* Chapter one

## See this course locally with docker
```bash
docker build -t course .
docker run -d --rm -p 80:8080 --name=course course
```
* After a few seconds, you can see the slides on http://localhost
* When you want to stop the instance, run:
```bash
docker stop course
```

## Print this course to pdf (only in chrome and chromium)
* Click on [this link](https://REPLACE_GITHUB_ACCOUNT.github.io/REPLACE_GITHUB_REPO_NAME/?print-pdf&pdfSeparateFragments=false)
* Then `CTRL+P` on the generated page
* Change the following settings

Setting | Value
--- | ---
Destination | Save as PDF
Pages | All
Pages per sheet | 1
Margins | Default
Options | Background graphics

* Click on save

## Edit this course
> For any question about Reveal.js usage, read [Reveal Documentation](reveal-documentation.md)

Feel free to submit as many pull request as you wish !

