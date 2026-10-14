# NEXT System Control — Development Portal

Public information site for [NEXT System Control](https://github.com/killernos/NEXT-System-Control). This repository is deliberately separate from the console application.

## Sections
- Current development focus: SSH, FTP and diagnostics
- Phase 1 reliability, Phase 2 user experience and future research roadmap
- Direct links to live GitHub commit history, pull requests, issues and published releases

## Publishing after review
1. Review and merge the pull request into `main`.
2. In **Settings → Pages**, choose **Deploy from a branch**.
3. Select `main` and `/ (root)`, then save.
4. The expected website is https://killernos.github.io/NEXT-System-Control-Website/.

## Editorial and safety policy
Roadmap and feature highlights are curated. Download links and latest-release
headings are refreshed from the public GitHub releases API. Never claim
functionality is verified or released before testing. Console binaries are
distributed from the release repository, not hosted by this static website.
Keep development branches isolated from the PS4 application repository.

## Required workflow for every release

An authorized release must update both the public
[release repository](https://github.com/killernos/NEXT-System-Control-Releases/releases)
and this website. Publication is not complete until both live surfaces agree.

1. Confirm the maintainer has tested the exact package on PS4.
2. Write detailed release notes covering actual additions, changes, and fixes,
   practical controls, and concise installation steps: download the PKG,
   install with the PS4 package installer, and launch NEXT System Control.
3. Use a direct statement such as "Tested on PS4 before release." Do not infer
   firmware compatibility from other releases or publish discouraging statements
   about missing test records. Do not add a generic "not a stable production
   release" disclaimer. Keep specific, actionable network-use guidance.
4. Publish the authorized package and notes to the public release repository.
   Verify the asset filename, size, and SHA-256, and preserve previous releases.
5. Update the release repository README and versioned notes. Update the website
   hero link, release section, highlights, testing summary, and latest-release
   card to the same version. Retain links to previous releases.
   Update `release-details`'s `data-release` tag as well: version-specific
   highlights, controls, testing results, and package details are hidden if
   the API finds a different version, so old details are never attached to
   a new download. The new release's introductory paragraph is shown instead.
6. Merge the public website and documentation changes after approval. This does
   not authorize merging the application development branch into its `main`.
7. Wait for GitHub Pages deployment and check the live website, public release
   notes, and download links. Do not report a branch preview as a live update.

The versioned release-notes document in the distribution repository is the
canonical copy for the public GitHub release body. Keep the source repository's
release body consistent when that release exists. No automatic publishing or
merging is enabled by this checklist.
