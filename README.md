# Kage

Kage is a minimalist Hugo theme inspired by the Tokyo Night color palette and the elegant simplicity of Shibui. Designed for developers and writers who love clean, dark, and subtle aesthetics, Kage provides a sleek, shadowy reading experience without distractions.

**Features:**

- Dark mode with Tokyo Night moon palette  
- Minimalist and distraction-free layout  
- Responsive and mobile-friendly design  
- Focus on typography and content clarity  
- Easy to customize and extend  

Perfect for blogs, portfolios, and technical documentation.

---

## Installation

Create your hugo site, cd into it and init a git.

```bash
hugo new site mysite
cd mysite
git init
```

Add Kage to your Hugo site:

```bash
git submodule add https://github.com/lairizzle/kage themes/kage
```
Set your theme in hugo.toml:
```toml
theme = "kage"
```

## Configuration
### Menus

```toml
[menus]
  [[menus.main]]
    name = 'Home'
    pageRef = '/'
    weight = 10

  [[menus.main]]
    name = 'Posts'
    pageRef = '/posts'
    weight = 20

  [[menus.main]]
    name = 'Tags'
    pageRef = '/tags'
    weight = 30

```

### Social Icons
To add social icons, you can indlude them in your hugo.toml:
```toml
[params.social]
  email        = "mailto:you@example.com"
  github       = "https://github.com/yourname"
  twitter      = "https://twitter.com/yourhandle"
  facebook     = "https://facebook.com/yourpage"
  linkedin     = "https://linkedin.com/in/yourname"
  youtube      = "https://youtube.com/@yourchannel"
  twitch       = "https://twitch.tv/yourchannel"
  instagram    = "https://instagram.com/yourname"
  mastodon     = "https://mastodon.social/@yourname"
  rss          = "/index.xml"
  gitlab       = "https://gitlab.com/yourname"
  bitbucket    = "https://bitbucket.org/yourname"
  discord      = "https://discord.com/users/yourid"
  telegram     = "https://t.me/yourname"
  threads      = "https://www.threads.net/@yourname"
  reddit       = "https://reddit.com/u/yourname"
  medium       = "https://medium.com/@yourname"
  dev          = "https://dev.to/yourname"
  stack-overflow = "https://stackoverflow.com/users/yourid"
  spotify      = "https://open.spotify.com/user/yourid"
  soundcloud   = "https://soundcloud.com/yourname"
  tumblr       = "https://yourblog.tumblr.com"
  vimeo        = "https://vimeo.com/yourname"
  goodreads    = "https://goodreads.com/yourname"
  paypal       = "https://paypal.me/yourname"

```
If you want to control the order you must make your own partial for footer.html and override the icon order.

### Shortcodes
There are shortcodes included for
- Spotify
```markdown
{{< spotify type="artist" id="63rbGTeN8Vr3DT0ZwveD0p" width="100%" height="380" >}}
```
- Steam
```markdown
{{< steam id="3138280" width="100%" height="200" >}}
```
- Github
```markdown
{{< github user="lairizzle" repo="kage" >}}
```
## Credits
Special thank you to https://github.com/ntk148v (Kien Nguyen-Tuan) for inspiration based on [Shibui](https://github.com/ntk148v/shibui). This theme was used as a reference for learning to build a clean hugo theme.
