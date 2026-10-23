# Decap CMS

The year site includes a Decap admin at `/admin/` so organisers can edit programme posts without writing YAML by hand.

Admin files live in the **year repository**, not in the Jekyll theme.

## Local editing

From the year repo:

```bash
npx decap-server
bundle exec jekyll serve
```

Then open `http://localhost:4000/sorrentoXXXX/admin/` (replace `XXXX` with the year, matching `baseurl`).

`local_backend: true` in `admin/config.yml` lets Decap write straight to the working copy. Commit and push as usual.

## Production

`admin/config.yml` uses the GitHub backend. Logging in from the published site needs a GitHub OAuth proxy (or [Decap Turbo](https://decapcms.org/docs/backends-overview/)). Until that is set up, use local Decap or the giki edit links.

When creating a new year, set:

```yaml
backend:
  name: github
  repo: lawrennd/sorrentoXXXX
  branch: main
```

in `admin/config.yml` to match that year's repository.

[Go back to main doc README.md](./README.md)
