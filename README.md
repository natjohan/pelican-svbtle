
# SVBTLE

Svbtle theme is a close copy of [Svbtle.com](http://www.svbtle.com) with
a few minor changes for use with [Pelican](http://pelican.notmyidea.org).

## DEMO

You can see the [theme in
action](http://williamting.com/drafts/this-is-a-theme-testing-post.html), or
the site code [here](https://github.com/wting/williamting.com).

![theme screenshot](https://raw.github.com/wting/pelican-svbtle/master/screenshot.png)

## FEATURES

- syntax highlighting for code blocks
- Google Analytics
- Disqus commenting
- custom list of links

## KNOWN ISSUES

- no IE testing
- no custom menu
- header date format is hardcoded in `./templates/header.html` with the
  exception of articles.
- Svbtle uses Freight-Sans-Pro for article titles and Proxima Nova for body.
  While they are two great fonts, neither are free. I've linked to them in
  case the client has them installed, but for users will be view the site
  with Open Sans.

## INSTALL

### FROM SOURCE

Download the [repository](https://github.com/wting/pelican-svbtle) and save
it somewhere accessible. Edit `settings.py` and modify the `THEME` variable
to point to the downloaded theme location.

### FROM OFFICIAL REPO

Please refer to Pelican theme [install
instructions](http://pelican.notmyidea.org/en/latest/pelican-themes.html).

## SETTINGS.PY

These are the Pelican global variables currently supported by the theme:

- `GOOGLE_ANALYTICS`
- `DISQUS_SITENAME`
- `LINKS(('name1', 'url1'), ('name2', 'url2'))`
- `DEFAULT_DATE_FORMAT = ('%b %d, %Y')`: suggested date format
- `FEED_DOMAIN = SITEURL`

When developing locally, set the following variable:

`SITEURL = http://localhost:8000`

## MODIFICATION

- Accent color can be changed by editing `@accent` in `./static/css/style.less`.

- A different Pygmentize theme can be used by editing `./Makefile` and
  running `make pygments`.

## QUICK ADDED BY NATJOHAN
twitter share button under articles
font-awesome icons
social links on sidebar 
inspired by [fjavieralba](http://fjavieralba.com/) and his flasky theme, thank to him !
Added global variables :
- `REVERSE_MAIL_USERNAME` : juste reverse your username for a little javascript obfuscation (ie: totogtr => rtgotot)
- `REVERSE_MAIL_HOST` : reverse like username example
- `LINKEDIN_URL`
- `GITHUB_URL`
- `FLICKR_URL`
- `TWITTER_USERNAME` : without @

## AUTHOR

William Ting

## LICENSE

Released under MIT License, full details in `LICENSE` file.
