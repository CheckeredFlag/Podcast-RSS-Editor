# Podcast RSS Editor
Started a [design podcast](https://anyway.fm/) couple of years ago, and in the very beginning,
I manually updated the RSS feed for every episode and very soon, I got sick of the 'tag dancing',
so tried a little bit building this tool, a very simple Podcast RSS editor in PHP for myself.

![](https://raw.githubusercontent.com/JJYing/Podcast-RSS-Editor/master/assets/screenshot.jpg)

Forked from https://github.com/JJYing/Podcast-RSS-Editor.  Many thanks to JJ Ying!

# 01. Features
- Add / Remove / Duplicate episodes from existing RSS feeds.
- Analyzing publish date and episode duration information.

# 02. Usage
- Copy the `example.xml` to a new file for each feed you want to maintain.
- Edit all the channel information for each file.
- Place the XML file in the `feeds` directory.
- Ensure all the XML files in `feeds` as well as the config.php have write permissions
  by the web server (e.g. chmod 666 config.php feeds/example.xml).
- To add and/or edit episodes, first select the desired feed in the '**Settings**' panel.

# 03. Authentication
 - There's a very simple authentication done with `.htaccess`, so all you gotta do is to generate
the `.htpasswd` file content [in this site](http://www.htaccesstools.com/htpasswd-generator/)
and replace it.
 - The parameter **AuthUserFile** of the `.htaccess` file is the path to the `.htpasswd` that
 **must to be the real path**. Be sure to change it as needed.
 - By default authentication is: user `admin` and password `admin`

# 04. Alternatives
- [Itunes podcast XML generator](http://codepen.io/jon-walstedt/pen/jsIup) by Jon Wålstedt
- [Podcast Generator](http://www.podcastgenerator.net/)
- Any Podcast hosting services.

# 05. Credits
- Some icons used are from the set [Squid Ink Line Icons](http://thesquid.ink/line-icons/)
