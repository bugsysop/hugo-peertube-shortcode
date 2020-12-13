# Hugo Peertube Shortcode

This is a shortcode for Hugo static site generator to include videos hosted on any Peertube instance. Peertube is a decentralized and federated video streaming and hosting platform: using  ActivityPub protocol for federation and P2P directly in the web browser for distributed downloading of data. 

### Install

Just copy the `peertube.html` file in the `layouts/shortcodes/` directory at the _root_ of your Hugo site. You have to create the `layouts` and `shortcodes` directories if they does not exist. You can learn more about _shortcodes_ from [Hugo documentation](https://gohugo.io/content-management/shortcodes/).

_That’s all Folks._

### Usage

Insert the _Shortcode_ in your Markdown content...

**Simplified syntax**  
Easy to use, but only default options.

```
{{< peertube vidcommons.org a547c41d-3f0e-4689-bb1c-44d533d16397 >}}
```

**Complete syntax**  
Give access to the complete set of options avaible for Peertube iframe.

```
{{< peertube host="indymotion.fr" id="a11de1b8-dbb2-4cef-9b1d-3f01e0af8425" title="0" >}}
```

| Params     | Comments                                                                        | Default |
| ---------- | ------------------------------------------------------------------------------- | ------- |
| `host`     | _Domain Name_ of instance: without `https://` nor training slatch (`/`)         | `None`  |
| `id`       | Identification _Code_ of the video (ex: `d49f95a9-b183-4f16-9341-8637ac3597ff`) | `None`  |
| `title`    | Display the video _Title_: `0` (no) or `1` (yes)                                | `0`     |
| `warning`  | Display a _Warning_ about privacy: `0` (no) or `1` (yes)                        | `0`     |
| `subtitle` | Display the video subtitle if exist: langage code (ex: `fr`)                    | `0`     |

Note: The default options are _hard coded_, if you want du change, you have to modify the source.

### Privacy

**1)** Peertube by itself use absolutely no cookies, no trackers.

**2)** The uses the BitTorrent P2P protocol to share bandwidth between users by default to help lower the load on the server induce that your IP address is being stored in the instance’s BitTorrent tracker as long as you download or watch the video For [more info](https://indymotion.fr/about/peertube#privacy) read this Peertube statement. 

### References

- [Peertube](https://joinpeertube.org/)
- [Hugo](https://gohugo.io)