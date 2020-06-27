# Amiga Website

_Currently Work in progress_

This site uses the Static Site Generator, Pelican.

[Get Pelican](https://blog.getpelican.com/)

## Installation
Make sure you have 

```
sudo apt install python3 python3-venv
```
Make a virtual env in a folder, and call env amigaweb and activate

```
python3 -m venv amigaweb
source amigaweb/bin/activate
```
Install wheel and pelican
```
pip install wheel pelican[Markdown]
```
Download the repo into a sub folder called **site**

or to make new pelcian site I ran ```pelican-quickstart```
## Generating Site
To generate static site run:
```
pelican content
```
To check site locally:
```
pelican --listen
```
## Push to GitHub and Subtree output

All of the project is in the master branch.

After generating the site everything should be push to master.

The output folder is setup as a subtree and set to gh-pages. Run:
```
git subtree push --prefix output origin gh-pages
```
This will update the publish version of the site on gh-pages branch.
