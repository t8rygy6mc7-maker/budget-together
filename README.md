# Even Keel — support & privacy

The public site for the Even Keel iPhone app (first published as Budget
Together, which is why the repository and its URLs still carry that name). Two
pages, served by GitHub Pages:

- `index.html` — the support page (Apple requires a Support URL)
- `privacy/index.html` — the privacy policy (Apple requires a Privacy Policy URL)
- `style.css` — shared styling for both

Plain HTML on purpose. No Jekyll, no theme, no front matter, no build step —
GitHub Pages serves these files exactly as they are, so there is nothing that
can silently fail to build between committing and a reviewer opening the link.

## Publishing

Settings → Pages → Source: **Deploy from a branch** → `main` → `/ (root)`.

The URLs are then:

```
https://<username>.github.io/budget-together/
https://<username>.github.io/budget-together/privacy/
```

Check both in a private window before submitting anything to App Review.

## Keeping the policy honest

The policy must keep matching what the app actually does. The version of record
is `PRIVACY.md` in the app repository; this HTML is the published copy of it. If
one changes, change the other — a published policy that contradicts the app is
worse than no policy at all.

Update the "Last updated" date at the top of `privacy/index.html` whenever the
text changes.
