# Sorrento Meeting Template Site

This is the template repository for the annual Sorrento Meeting, held at the Grand Hotel Vesuvio, Sorrento, Italy.

Year sites use the shared remote theme [`lawrennd/jekyll-theme`](https://github.com/lawrennd/jekyll-theme) with `style: sorrento`. Do not point a new year at the personal `cabrerac/jekyll-theme-sorrento` fork.

## Creating a New Year's Site

**These steps need to be done by someone with admin access to the `lawrennd` GitHub organisation.**

1. Create the new repo in GitHub by going to <https://github.com/new>, use the name `sorrentoXXXX` where `XXXX` is the year of the meeting (e.g. `sorrento2028`).

2. Select "Create from Template" and use `lawrennd/sorrento-template` as the template.

3. Give the repo a description, e.g. `"The Sorrento Meeting 2028"`.

4. Make sure the repo is set to **public**.

5. Create the repo.

6. Edit `_config.yml` in the new repo:
   - Replace all occurrences of `XXXX` with the meeting year.
   - Update `subtitle` with the meeting theme.
   - Update `conference.dates` with the exact meeting dates (include the Sunday welcome day when it is advertised).
   - Set `ghub.branch` to the default branch (`main`).
   - Update `conference.chairs` with the names of the organising committee.
   - Update `author.email` with the contact email.

7. Edit `admin/config.yml` and set `backend.repo` to `lawrennd/sorrentoXXXX`.

8. Edit `index.html` to describe the meeting programme (workshops, plenary topics etc.).

9. Edit `submission.html` with the call for abstracts and submission deadline, if applicable.

10. Add programme posts to `_posts/`. See the example post `_posts/XXXX-MM-DD-workshop-example.md` and recent meetings for reference.

11. In the GitHub repository settings, go to **Pages** and set the source to **GitHub Actions**.

12. The site will be published at `https://lawrennd.github.io/sorrentoXXXX/` once the first build completes.

## Site Structure

| File / Directory | Purpose |
|---|---|
| `_config.yml` | Main configuration — update year, dates, chairs, theme |
| `index.html` | About / home page — describe the meeting |
| `program.html` | Programme overview — auto-generated from `_posts/` |
| `accommodation.html` | Venue and activities info — **reusable, rarely needs changing** |
| `getting-there.html` | Travel info from Naples airport — **reusable, rarely needs changing** |
| `registration.html` | Registration instructions |
| `submission.html` | Call for abstracts / submissions |
| `_posts/` | One file per programme session (workshops, plenary, etc.) |
| `_layouts/program.html` | Local override for the programme overview layout |
| `admin/` | Decap CMS for programme editing |
| `assets/images/` | Banner and map images |
| `doc/` | Organiser documentation and checklists |

## More Information

- [Organiser documentation](doc/README.md)
- [Decap admin](doc/decap.md)
- [Past meeting sites](https://github.com/lawrennd/)
- [Jekyll documentation](https://jekyllrb.com/docs/)
- [Remote theme source](https://github.com/lawrennd/jekyll-theme)
- [GitHub Pages documentation](https://docs.github.com/en/pages)
