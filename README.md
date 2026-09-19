# w7yfr.github.io

The front door. One static page, no build step — what is in `index.html` is
what gets served.

It is a *user site*, which is the one repository name GitHub treats specially:
because it is called `<username>.github.io` it serves at the root rather than
under a path. That also makes it the place a custom domain is attached, and
attaching one there moves every project site under it — `cwt` becomes
`<domain>/cwt/` with nothing to change in the `cwt` repository.

The palette and the wordmark treatment are lifted from
[cwt](https://github.com/W7YFR/cwt) so the index and the things it indexes read
as one site. If the colors change there, change them here too — they are
duplicated on purpose, since a shared stylesheet across two independently
deployed repositories is a coupling that buys nothing at this size.

## Serving it locally

Any static server will do; there is nothing to compile.

```
python3 -m http.server 8000
```
