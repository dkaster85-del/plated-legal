# plated-legal

**This repo no longer holds any documents.** It exists only to keep
`legal.plated-fitness.com` alive as a set of redirects.

The privacy policy and terms of use now live in
[plated-site](https://github.com/dkaster85-del/plated-site) and are served from
the main domain:

| Old URL                                     | Now redirects to                        |
| ------------------------------------------- | --------------------------------------- |
| `legal.plated-fitness.com/privacy/`          | `plated-fitness.com/privacy/`           |
| `legal.plated-fitness.com/terms/`            | `plated-fitness.com/terms/`             |
| `legal.plated-fitness.com/`                  | `plated-fitness.com/`                   |

They were split across two domains originally; consolidating them means one
repo, one deploy, and one URL a link can point at. The subdomain is kept
because its privacy-policy URL was given to App Store Connect and is compiled
into builds already out with testers — retiring it would break those.

**Do not add documents here.** The source of truth is `legal/*.html` in the
private app repo, published into `plated-site` by `scripts/publish-legal.js`.

Because GitHub Pages serves static files only, these are meta-refresh redirects
with a `rel=canonical` rather than real 301s — that is the closest a Pages site
can get.
