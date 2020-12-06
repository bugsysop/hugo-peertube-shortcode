# Hugo Peertube Shortcode

Peertube is a decentralized and federated video streaming and hosting platform, using  ActivityPub protocol and P2P directly in the web browser. This is a shortcode for Hugo static site generator to include videos hosted on any Peertube instance.

### Install

Just copy the `peertube.html` file in the `layouts/shortcodes/` directory at the _root_ of your Hugo site. Create the `layouts` and `shortcodes` directories if they does not exist. You can learn more about _shortcodes_ from [Hugo documentation](https://gohugo.io/content-management/shortcodes/).

That’s all Folks.

### Usages

Insert in your Markdown content...

Option 1:

```
{{< peertube vidcommons.org a547c41d-3f0e-4689-bb1c-44d533d16397 16by9 >}}
```

Option 2:

```
{{< peertube host="indymotion.fr" id="a11de1b8-dbb2-4cef-9b1d-3f01e0af8425" >}}
```

### References

- [Peertube](https://joinpeertube.org/)
- [Hugo](https://gohugo.io)