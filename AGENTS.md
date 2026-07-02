# AGENTS.md

## Cursor Cloud specific instructions

This repository is a **GitHub profile README** repo (for the user `cardoso-ix`). It is not an application:

- The only tracked file is `README.md`. There is no `package.json`, lockfile, source code, test suite, build system, or dependency manifest.
- The "product" is the Markdown profile that GitHub renders on the user's profile page. The development loop is: edit `README.md`, then preview the rendered Markdown.
- There is nothing to install for the repo itself, and there are no lint/test/build commands defined by the project.

### Previewing the README (GitHub-Flavored Markdown)

To preview how the README renders (tables need GFM), use a Markdown renderer with the `tables` extension, e.g. Python's `markdown` package:

```
python3 -m pip install --quiet markdown
python3 -m markdown -x tables -x fenced_code README.md > /tmp/readme.html
# then serve and open:
python3 -m http.server 8080   # (run from the directory containing the HTML)
```

Note: plain CommonMark renderers will not render the `Projetos em destaque` table — always enable the `tables`/GFM extension when previewing.
