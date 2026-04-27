A basic blog website using [hugo](https://github.com/gohugoio/hugo) as framework, and [hugo-PaperMod](https://github.com/adityatelange/hugo-PaperMod) as the website's theme.

### Prerequisites

- Hugo v0.153.2
- Git 2.49.0 (or latest)

### Cloning hugo-PaperMod (if it didn't work)

Run this command in the root folder of site:

```bash
git submodule update --init --recursive
```

hugo-PaperMod should be cloned automatically to `./themes/PaperMod/`.

### Updating hugo-PaperMod

Go to root folder of site, then run this command:

```bash
git submodule update --remote --merge
```

Then rebuild site using command:

```bash
hugo
```

### Deployment

Deploy the website locally via localhost:

```bash
hugo server
```

The website will be hosted at `http://localhost:1313/`.

> [!NOTE]
> To build website before deploying to the server, use
> 
> ```bash
> hugo
> ```
>
> so `<link>` tags in /public directory will refer to the `baseURL` in the config, not using `localhost:1313`.

> Apparently you don't need to rebuild the page if you already setup an actions.
