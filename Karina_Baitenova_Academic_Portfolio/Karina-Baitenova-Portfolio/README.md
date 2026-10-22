# Karina Baitenova

A personal website for software engineering, application security, and graduate research preparation.

The site is built with Jekyll 4.4 and the al-folio v1.0.15 theme. It keeps the familiar academic site layout while using Karina's own writing, research direction, project plans, navigation, and visual identity.

## Pages

- `about.md`: introduction and study direction
- `projects.md`: CommitGuard, FuzzRoute, AuthAudit, and a proposed capstone
- `research.md`: research questions and graduate study plans
- `publications.md`: honest publication status
- `repositories.md`: code and repository links
- `cv.md`: short academic profile
- `blog.md`: notes and topics

See `SETUP_FOR_KARINA.md` for first-time deployment, portrait replacement, and checks.

## Development

```bash
bundle install
bundle exec jekyll doctor
bundle exec jekyll build --trace
bundle exec jekyll serve --host 0.0.0.0 --port 4000 --force_polling --watch
```

## Credits

Site layout and theme architecture: [al-folio](https://github.com/alshedivat/al-folio) and its open-source ecosystem. Adapted from an existing customized portfolio with permission. Keep license and dependency notices intact.
