## Installation

```
$ cd /<your-hugo-site-directory>
$ git submodule add https://github.com/MythalCorp/hugo-mythalcorp-theme.git themes/hugo-mythalcorp-theme
```



## Configuration

Edit `hugo.toml`

```
baseURL = 'https://mythalcorp.github.io/'
languageCode = 'fr'
title = 'Mythal Corp Site'
theme = "hugo-mythalcorp-theme"
```

[config.yaml](https://github.com/miguelsimoni/hugo-8bits-theme/blob/main/exampleSite/config.yaml)

### Multilingual

You can show or hide the Languages dropdown menu from `config.yaml`:

```yaml
languagesMenuEnabled: true
```

### Breadcrumb

You can show or hide the current page in the breadcrumb from `config.yaml`:

```yaml
breadcrumb:
  showCurrent: true
```

### Pagination Loader

You can enable or disable the pagination loader (Load More button) in the list pages from `config.yaml`:

```yaml
pagination:
  loader: true
```

Disabling it will show the standard pagination widget.

### Background

You can set a theme background just dropping an image on the `static/images/` folder and typing its name on the `params.background.image` parameter. Also you can set a parallax effect and its speed for the posts section.

```yaml
background:
  image: "../images/background.png"
  parallax: true
  speed: 10
```

### Contact

You can enable de Contact form to let visitors send you messages using a message service like [Formspree](https://formspree.io/) just adding your contact form action URL in `config.yaml`:

```yaml
contact:
  formAction: https://formspree.io/f/yourformcode
```

### Social Networks

You can add the usernames for the current supported social networks in `config.yaml`:

```yaml
social:
  - network: twitter
    link: "https://www.twitter.com/8bits"
  - network: facebook
    link: "https://www.facebook.com/8bits"
  - network: instagram
    link: "https://www.instagram.com/8bits"
```

See [config.yaml](https://github.com/miguelsimoni/hugo-8bits-theme/blob/main/exampleSite/config.yaml) for more examples on social networks parameterization.

### Comments

Powered by [Disqus](https://disqus.com)

```yaml
disqusShortname: "yourdiscussshortname"
```

Disable the comments system by leaving `params.disqusShortname` empty.

### Google Analytics

```yaml
googleAnalytics: "UA-123-45"
```

Disable the Google Analytics by leaving `params.googleAnalytics` empty.

### More Settings!

See the whole configuration in the [config.yaml](https://github.com/miguelsimoni/hugo-8bits-theme/blob/main/exampleSite/config.yaml) file.


## Example Site

The [`exampleSite`](https://github.com/miguelsimoni/hugo-8bits-theme/tree/main/exampleSite) folder is based on [Hugo Basic Example](https://github.com/gohugoio/hugoBasicExample) and offers an example site for this theme.

The `exampleSite/content/` folder contains the following:

- A section called `/post/` with sample markdown content.
- An `about.md` that is intended to provide the `/about/` page for a theme demo.
- A `contact.md` that is intended to provide the `/contact/` page for a contact form.


## Almost there...

In order to see your site in action, you can run Hugo's built-in local server.

```bash
$ cd exampleSite
$ hugo server -t ../..
```

Now enter [`http://localhost:1313/`](http://localhost:1313/) in the address bar of your browser.


## Deployment

- [Hosting on GitHub](https://gohugo.io/hosting-and-deployment/hosting-on-github/)
- [More hosting and deployment options](https://gohugo.io/hosting-and-deployment/)


## Contributing

- Found a bug?
- Got an idea for a new feature?

Let me know it using the [issue tracker](https://github.com/miguelsimoni/hugo-8bits-theme/issues) or make it directly with a [pull request](https://github.com/miguelsimoni/hugo-8bits-theme/pulls).


## License

This theme and the framework that made it possible are released under the MIT License. Check the [original framework license](https://github.com/nostalgic-css/NES.css#copyright-and-license) for additional licensing information.


## Thanks

Thanks to [Steve Francia](https://github.com/spf13) for creating Hugo and the awesome community around the project. And also thanks to [BcRikko](https://github.com/BcRikko) for creating this awesome nostalgic framework.
