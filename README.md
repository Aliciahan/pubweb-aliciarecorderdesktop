# Alicia Recorder — public pages

The website of Alicia Recorder for macOS, published with GitHub Pages at
https://aliciahan.github.io/pubweb-aliciarecorderdesktop/ :

| Page | File | Address |
|---|---|---|
| Home: what the app is, in English and Chinese | `index.md` | `/` |
| Privacy policy (also the app's and the App Store's privacy policy address) | `privacy.md` | `/privacy/` |
| Support: how to get help, common questions | `support.md` | `/support/` |

Plain Jekyll as GitHub Pages runs it: one layout (`_layouts/default.html`), one stylesheet (`assets/style.css`),
kramdown, no theme and no plugins of our own. The pages load nothing from other servers: no web fonts, no scripts, no
analytics, no images hosted elsewhere, no cookies. Keep it that way; the privacy policy (section 10) says so.

## `privacy.md` is generated

Do not edit `privacy.md` here. Its text comes from the app's repository, `docs/store/privacy-policy.md`, the only
source of the policy. There, `scripts/site-sync.sh` writes this file: it keeps the part after the draft's
`policy:begin` line, drops the developer notes and the source comments, adds the front matter and the
English/Chinese anchors, and refuses while a placeholder is left. To change the policy, change the draft, run the
script, and commit both repositories.

## Publishing

Commit and push the `gh-pages` branch; GitHub Pages builds the site from the branch root. If the site does not
appear after the first push, turn it on in the repository's Settings › Pages: “Deploy from a branch”, branch
`gh-pages`, folder `/ (root)`. Check the build under the repository's Actions tab.

Commits here are public: use GitHub's noreply address for them, and put nothing private in the pages (no email
address, no real name, no paths from your Mac). Questions from users go to this repository's Issues, which are public
too.
