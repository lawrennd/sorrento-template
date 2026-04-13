# Sorrento Meeting Template Site

This is the template repository for the annual Sorrento Meeting, held at the Grand Hotel Vesuvio, Sorrento, Italy.

## Creating a New Year's Site

**These steps need to be done by someone with admin access to the `lawrennd` GitHub organisation.**

1. Create the new repo in GitHub by going to <https://github.com/new>, use the name `sorrentoXXXX` where `XXXX` is the year of the meeting (e.g. `sorrento2027`).

2. Select "Create from Template" and use `lawrennd/sorrento-template` as the template.

3. Give the repo a description, e.g. `"The Sorrento Meeting 2027"`.

4. Make sure the repo is set to **public**.

5. Create the repo.

6. Edit `_config.yml` in the new repo:
   - Replace all occurrences of `XXXX` with the meeting year (e.g. `2027`).
   - Update `subtitle` with the meeting theme.
   - Update `conference.dates` with the exact meeting dates.
   - Update `conference.chairs` with the names of the organising committee.
   - Update `author.email` with the contact email.

7. Edit `index.html` to describe the meeting programme (workshops, plenary topics etc.).

8. Edit `submission.html` with the call for abstracts and submission deadline, if applicable.

9. Add programme posts to `_posts/`. See the example post `_posts/XXXX-MM-DD-workshop-example.md` and the 2026 meeting for reference.

10. In the GitHub repository settings, go to **Pages** and set the source to **GitHub Actions**.

11. The site will be published at `https://lawrennd.github.io/sorrentoXXXX/` once the first build completes.

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
| `assets/images/` | Banner and map images |
| `doc/` | Organiser documentation and checklists |

## More Information

- [Past meeting sites](https://github.com/lawrennd/)
- [Jekyll documentation](https://jekyllrb.com/docs/)
- [Remote theme source](https://github.com/cabrerac/jekyll-theme-sorrento)
- [GitHub Pages documentation](https://docs.github.com/en/pages)
