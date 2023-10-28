# CEFI website

This repo contains code for the CEFI website, built using <a href="https://quarto.org/" target="_blank">Quarto</a>.

## Files

The website is built on three main types of files:
* Configuration file
* Website pages
* Styling files

### Configuration file

<p>Quarto website options are defined in a configuration file called <code>_quarto.yml</code>.</p>
<p>The configuration file should be edited to add new menu items to the top-navigation bar.</p>

### Website pages

<p>In Quarto, website pages are defined by individuals files with extension <code>.qmd</code>.</p>
<p>Each .qmd file should begin with a YAML code, followed by the page content written in HTML and/or Markdown.</p>

### Styling

<p>The CEFI website uses a base Quarto theme along with custom SCSS and CSS styling.</p>
<p>SCSS should be used to costumize the base theme, using the file <code>custom.scss</code>.</p>
<p>CSS should be used to set the global style for the HTML components in the website, using the file <code>styles.css</code>.</p>
<p>If a page requires specific changes relative to the global styling, then CSS code should be added to the respective page following the YAML code and within the <code><style></style></code> tags.</p>
