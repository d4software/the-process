---
layout: page
title: Development Process
desc: "Practices we follow while developing software."
permalink: /development/
---

## Development Process

This is list of practicies that we follow while developing software:

 * Projects are versioned using the approach outlined at [http://semver.org]()
 * We _broadly_ follow the [Gitflow](http://nvie.com/posts/a-successful-git-branching-model/) model, with development occuring in the "develop" branch, with "master" being deployable at any time.
 * While development is progressing, developers can optionally maintain a changelog file at the root of the repo. At the end of release, the changelog is completed and/or tidied up, this doubles up as the release notes, which may be email out to customers. We follow the format outlined at [http://keepachangelog.com/]().
