# 4nimesh.github.io

Personal website of Animesh Sarkar, built with Jekyll and served by GitHub Pages.

## Where to edit things

| To change… | Edit this file |
|---|---|
| Name, position, email, profile links (Scholar, arXiv, ORCID, MathSciNet), menu | `_config.yml` |
| The "About" text on the home page | `index.md` |
| Papers (published and submitted) | `_data/publications.yml` |
| Talks, conferences, schools and workshops | `_data/events.yml` |
| Courses on the Teaching page | `_data/teaching.yml` |
| MA111 tutorial sheets | `ma111.md` (PDFs go in `assets/ma111/`) |
| Colours, fonts, spacing | `assets/css/site.css` |

Each data file has a short comment at the top showing the format. Add new items at the top of
the list; the pages group them by year automatically.

To show an arXiv, ORCID or MathSciNet link, paste the URL after `url:` in `_config.yml`.
Links with an empty `url:` are hidden.

Maths on a page: add `math: true` to the page's front matter and write `$...$` as usual.
