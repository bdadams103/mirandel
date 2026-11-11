# Working on Mirandel

The live site (Mirandel.netlify.app) deploys automatically from `main`.
Nothing goes to `main` without Ben looking at it first.

## The rule

1. **Never commit directly to `main`.** All work happens on a branch,
   named `draft/<short-description>` (for example `draft/ferry-falls-towns`).
2. **Push the branch.** Netlify builds a Deploy Preview for the branch,
   which is a live copy of the site at a unique preview URL. That URL is
   the thing to review, not the code diff.
3. **Ben reviews the preview.** He checks how it looks and plays in the
   browser, and says go or asks for changes.
4. **Merge only after approval.** The branch merges into `main` through a
   pull request, after Ben says go. Merging is what publishes to the live
   site.

## Enforcement

- GitHub branch protection on `main` (Settings, Branches): require a pull
  request before merging, block direct pushes. This makes the rule
  mechanical instead of a promise. If it is not turned on yet, turn it on
  before the next change.
- Netlify Deploy Previews must stay on (Site settings, Build and deploy,
  Deploy Previews). If a branch push does not produce a preview URL,
  stop and fix that before merging anything.

## If a preview looks wrong

Fix it on the same branch and push again. The preview URL updates.
Do not merge a branch whose preview has not been reviewed.
