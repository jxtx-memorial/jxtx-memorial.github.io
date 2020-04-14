# Readme

This repo was forked from the starter website repo for the [Forty theme](https://github.com/andrewbanchich/forty-jekyll-theme). I've also created a Github account for the [jxtx memorial email](https://github.com/jxtx-memorial), which is where we'll eventually publish the website officially, but I figured we could work on it from here for now and then just move all the docs over.

# Guide to useful files in this repo

## Website formatting

`_includes` - HTML files for formatting of website elements that appear on every page. Mostly I've been changing `header.html` and `footer.html`. `head.html` is also important but I haven't tried modifying it yet. `tiles.html` is for formatting "tiles" that can appear on the home page (you can look at the [Forty sample website](https://andrewbanchich.github.io/forty-jekyll-theme/) to see what I mean) - I didn't want to deal with these, but we can potentially modify the home page in the future to include this.

`_layouts` - HTML files for formatting of specific page styles. I use `page.html` as the formatting for the memorials page, and `home.html` as the formatting for the homepage. `landing.html` is also nice.

`_posts` - docs in here don't show up on the actual website. I put two sample page templates here that I got from forking the repository (`elements.md`, `landing.md`). Super useful for looking at formatting examples.

`_sass/layout` - CSS files for formatting of some components.

`assets` - images, some more CSS files, javascript (`js` plugins) that we can leave alone.

## Website content

`_config.yml` - place to put website-wide info (email, title, etc.).

`index.md` - content for the website's home page. It says `md` but I ended up writing it in HTML.

`memorials.md` - template for student/faculty submissions about James.

## Things we don't need to touch

`.gitignore` - add files you don't want Git to track.

`Gemfile` - for jekyll, we can leave this alone for now.

`forty_jekyll_theme.gemspec` - more jekyll stuff that we can ignore.

It seems like any markdown (`.md`) or HTML (`.html`) docs we end up adding to this main repository will be added to the website as separate pages, and automatically incorporated into the navigation. So that's how we create new pages.