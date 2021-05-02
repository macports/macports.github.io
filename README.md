# macports.github.io

This repository contains the news posts available at [www.macports.org/news](https://www.macports.org/news/).

## Testing changes locally

You should test any changes to the web site locally before pushing.

In the Terminal, `cd` to the root directory of your clone.

### Install Ruby and the GitHub Pages gems

[GitHub Pages currently uses Ruby 2.7.x](https://pages.github.com/versions/) so install ruby27 with MacPorts:

    sudo port install ruby27

Install the bundle of gems specified by this project's Gemfile:

    bundle2.7 install

The gems will be installed in the vendor/bundle subdirectory of the current directory.

If it's been awhile since you installed the bundle, update it:

    bundle2.7 update

### Test the web site

Start a local web server by running:

    bundle2.7 exec jekyll serve --baseurl ''

Now you can access <http://127.0.0.1:4000/news/> in your web browser to see the web site. When you make changes to your clone, your local site will automatically update. When done testing, press <kbd>Ctrl</kbd> + <kbd>C</kbd> to stop the local web server.

Changes to \_config.yml are not automatically reflected. If you change \_config.yml, stop and start the local web server to see those changes take effect.

---

These instructions are based on [GitHub's instructions](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/).
