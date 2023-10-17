# Content Website Template (aka. _churrificator_)

A template for one-click content websites.

To get the site online:

1. Sign up for an account at [Netlify](https://netlify.com)
2. Import the GitHub project here: <https://app.netlify.com/start> and accept the default settings
3. Optional: Register a nice domain at [NameCheap](https://namecheap.com) and link the domain to the Netlify project

Customize the site by changing these:

- Site URL at `CNAME`
- Site metadata at `_config.yml`
- Publish workflow at `.github/workflows/publish.yml`
- Main color at `assets/css/style.scss`
- Logos at `assets/*.png` (Figma template at <https://www.figma.com/file/dxdUwTexPQeWiHiOTECzVl/Churriweb-Template>)

## Development

Use Docker and save yourself a headache. Right-click `docker-compose.yml` on Visual Studio Code and select "Compose Up". Or run this from Terminal:

```sh
docker run --rm --volume="$PWD:/srv/jekyll" --publish 4000:4000 jekyll/jekyll jekyll serve
```

## TODO

- [ ] Disable pagination plugin
