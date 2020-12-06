# Hugo Peertube Shortcode

Peertube is a decentralized and federated video streaming and hosting platform, using  ActivityPub protocol and P2P directly in the web browser. This is a shortcode for Hugo static site generator to include videos hosted on any Peertube instance.

### Install

Just copy the `peertube.html` file in the `layouts/shortcodes/` directory at the _root_ of your Hugo site. Create the `layouts` and `shortcodes` directories if they does not exist. You can learn more about _shortcodes_ from [Hugo documentation](https://gohugo.io/content-management/shortcodes/).

That’s all Folks.

### Usage

Insert in your Markdown content...

Option 1: simplified syntax

```
{{< peertube vidcommons.org a547c41d-3f0e-4689-bb1c-44d533d16397 >}}
```

Option 2: complet set of options avaible for Peertube iframe.

```
{{< peertube host="indymotion.fr" id="a11de1b8-dbb2-4cef-9b1d-3f01e0af8425" >}}
```

| Params     | Comments                                                                        |
| ---------- | ------------------------------------------------------------------------------- |
| `host`     | _Domain Name_ of instance: without `https://` nor training slatch (`/`)         |
| `id`       | Identification _Code_ of the video (ex: `d49f95a9-b183-4f16-9341-8637ac3597ff`) |
| `class`    | Replace the hard coded `style` with your own custom CSS `class`                 |
| `title`    | Display the video _Title_: `0` (no, default) or `1` (yes)                       |
| `warning`  | Display a _Warning_ about privacy: `0` (no, `default`) or `1` (yes)             |
| `subtitle` | Display the video subtitle if exist: langage code (ex: `fr`)                    |

Note: by default the Title and the Warning notice are set to _no_. These options are _hard coded_, if you want du reverse this, you have to modify the source.

### References

- [Peertube](https://joinpeertube.org/)
- [Hugo](https://gohugo.io)