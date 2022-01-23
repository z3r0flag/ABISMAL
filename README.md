# ABISMAL - A Big Informational Site Management Algorithm

### What is it?
ABISMAL aims to make managing a large website easy! Just write bare html pages without worrying about metadata or navbar organisation. The navbar and metadata for every page get dynamically and automatically updated with every addition you make to your website.

### How to use it?
* Put bare .html files in the 'pages' directory (do not include DOCTYPE or head/body/main tags).
* Unless you want specific capitalisation in your navbar (e.g. a page called 'GPG Key'), do not capitalise your .html files. A file called 'index.html' will appear as 'Index' in the navbar. If your navbar entry needs to have spaces in it, name the file like so: 'example_file.html'.
* Make sure you have a file called `ABISMAL.conf` in the root directory of your website. The layout of this file is simple:

```
sitename=name of site
language=2 letter language code (e.g. en)
backgroundimage=path to background image (e.g. images/background.png)
backgroundcolor=hex code or color name, just like in html
```

* Styles which are applied to all pages are in `global.css`.
* Run `./mksite` to build the website.

### How to set up my .gitignore?
Put the following content into your .gitignore if you are deploying the site to a git repository:

```
pages/
ABISMAL.conf
README.md
mksite
```
