# CEFI website

This repo contains code for the CEFI website, built using <a href="https://quarto.org/" target="_blank">Quarto</a>.

Here, we provide an overview of how to contribute to the building of the website, including:
* [Files](https://github.com/CanadianEFI/website/edit/main/README.md#files)
* [Folder structure](https://github.com/CanadianEFI/website/edit/main/README.md#folder-structure)
* [Protected branches & Pull requests](https://github.com/CanadianEFI/website/edit/main/README.md#protected-branches--pull-requests)

<br>

## Files

The website is built on three main types of files:
* [Configuration file](https://github.com/CanadianEFI/website/edit/main/README.md#configuration-file)
* [Website pages](https://github.com/CanadianEFI/website/edit/main/README.md#website-pages)
* [Styling files](https://github.com/CanadianEFI/website/edit/main/README.md#styling)

<p>Changes should only be made to the files at the root of the the website directory (<i>i.e.</i>, <code>/website</code>).</p>

### Configuration file

<p>Quarto website options are defined in a configuration file called <code>_quarto.yml</code>.</p>
<p>The configuration file should only be edited to add new menu items to the top-navigation bar.</p>

### Website pages

<p>In Quarto, a website page is defined by a file with extension <code>.qmd</code>.</p>
<p>Each .qmd file should begin with a YAML code, followed by the page content written in HTML and/or Markdown.</p>

### Styling

<p>The CEFI website uses a base Quarto theme along with custom SCSS and CSS styling.</p>
<p>SCSS should be used to customize the base theme, using the file <code>custom.scss</code>.</p>
<p>CSS should be used to set the global style for the HTML components in the website, using the file <code>styles.css</code>.</p>
<p>If a page requires specific changes relative to the global styling, then CSS code should be added to the respective page following the YAML code and within the <code><style></style></code> tags.</p>
<p>Styling within an HTML element should be kept to a minimum, only when absolutely necessary.</p>

<br>

## Folder structure

The repo contains two types of folders:
* [Automatically updated](https://github.com/CanadianEFI/website/edit/main/README.md#automatically-updated-folders)
* [Editable](https://github.com/CanadianEFI/website/edit/main/README.md#editable-folder)

### Automatically updated folders

<p>All but one folder (<code>_assets</code>) in this repo should remain unedited.</p>
<p>The folders <code>_site</code>, <code>.quarto</code>, and <code>docs</code> contain the documents required to render the website. These folders are configured to update automatically when changes made to the files at the root of the website directory are committed and pushed to the repo.</p>

### Editable folder

<p>The only folder that contributors may add to is the <code>_assets</code> folder.</p>
<p>The <code>_assets</code> folder stores the fonts and images used in the website.</p>
<p>Therefore, when adding new images to the website, these should be saved in the <code>_assets</code> folder.</p>

<br>

## Protected branches & Pull requests

<p>The main branch is protected. Therefore, all commits must be made to a non-protected branch and submitted via a pull request before changes can be merged into the main branch. All pull requests will be reviewed and approved by the repo Admin.</p>

### Naming branches
<p>When creating a new branch, name it with your initials followed by the section of the website you are contributing to (<i>e.g.</i>, crf-homepage).</p>
<p>If the changes you are making span more than one page, add a short description of the task instead (<i>e.g.</i>, crf-updating-past-events).</p>
<p>When naming branches, use lower case and hypen to separate words.</p>

<br>

## Summary

* Only files at the root directory should be edited.
* When adding images to the website, save them into the <code>_assets</code> folder.
* Upon commit, the website is automatically rendered and updated.
* Commits must be made to a non-protected branch and submitted via a pull request. 
* Pull request will be reviewed and approved by the repo Admin.

<br>
