---
layout: page
hide_hero: true
---
This is a place for random development notes that can be removed once we're in good shape.

## Overriding the Theme
The theme is installed via a gem. What this means is that the theme files don't actually exist in the repository. You *can* still override them. In order to do so, find the component you want to edit/override in the [main repository](https://github.com/chrisrhymes/bulma-clean-theme) and create a corresponding file here.

For example, if you want to add some content to the footer in a way other than the [footer menu](http://www.csrhymes.com/bulma-clean-theme/docs/navigation/footer-navigation/), go find the footer template. That's [this file](https://github.com/ercjns/jn2020/blob/master/_includes/footer.html) which has a path of `_includes/footer.html`. Create that file (and the parent folder if it doesn't exist yet) and copy the contents locally. Make your changes, and save. When you refresh the site, jekyll will use the overridden template file rather than the file from the gem.

If that didn't make any sense, maybe the [documentation](http://www.csrhymes.com/bulma-clean-theme/docs/getting-started/theming/) is better

## Markdown
If you're not familiar with markdown, it's basically a syntax for **SUPER** lightweight html. In Jekyll you can mix in <strong>actual</strong> html as well, but I'd generally try to avoid that. [This](https://www.markdownguide.org/basic-syntax/) is a pretty good basic reference.