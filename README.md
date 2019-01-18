![Version](https://img.shields.io/badge/version-v1.0.0-blue.svg)
![CircleCI](https://img.shields.io/circleci/project/github/Fried-Chicken/news-outlet/master.svg)
![Issues](https://img.shields.io/github/issues/Fried-Chicken/news-outlet.svg)
![License](https://img.shields.io/github/license/Fried-Chicken/news-outlet.svg)
![Stars](https://img.shields.io/github/stars/Fried-Chicken/news-outlet.svg)
![Forks](https://img.shields.io/github/forks/Fried-Chicken/news-outlet.svg)
# News Outlet
This is a theme created to look like news outlets for [ghost](http://github.com/tryghost/ghost/) blogs. This is the latest development version of News Outlet. If you're just looking to download the latest release, head over to the [releases](https://github.com/Fried-Chicken/news-outlet/releases) page.

&nbsp;

![screenshot-desktop](./assets/screenshot-desktop.jpg?raw=true)

&nbsp;

# Demo Site
Vist the demo site [here](https://fried-chicken.github.io/news-outlet/)

# Templating
Ghost uses [Handlebars](http://handlebarsjs.com/) for its themes.

**The main files are:**
- `default.hbs` - The main template file
- `index.hbs` - Used for the home page
- `post.hbs` - Used for individual posts
- `page.hbs` - Used for individual pages
- `tag.hbs` - Used for tag archives
- `author.hbs` - Used for author archives

# Development

News Outlets styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
$ yarn install
$ yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
$ yarn zip
```

# PostCSS Features Used

- Autoprefixer - Don't worry about writing browser prefixes of any kind, it's all done automatically with support for the latest 2 major versions of every browser.
- Variables - Simple pure CSS variables
- [Color Function](https://github.com/postcss/postcss-color-function)


# SVG Icons

News Outlet uses inline SVG icons, included via Handlebars partials. You can find all icons inside `/partials/icons`. To use an icon just include the name of the relevant file, eg. To include the SVG icon in `/partials/icons/rss.hbs` - use `{{> "icons/rss"}}`.

You can add your own SVG icons in the same manner.


# License
Released under the [MIT license](LICENSE).
