---
layout: default
title: Pull Requests
nav_order: 11
---

<!-- prettier-ignore-start -->

# Pull Requests
{: .no_toc }

- Mechanism to propose changes to a repo and facilitate discussion about them.

- The project maintainers, and potentially other contributors, can:

    - Review the changes

    - Comment on them

    - Suggest modifications

    - Approve or close the request

- Pull requests are not part of git proper.

- They are facilitated by git hosting solutions like GitHub.

## Table of Contents
{: .no_toc }

1. TOC
{:toc}

<!-- prettier-ignore-end -->

## Creating Pull Requests

Pull requests are opened via the GitHub.com page for the repository.

Git GUIs (like Visual Studio) will often provide you with a link to create a request after pushing changes to a remote branch.

## Pull Request Merge Conflicts

You will be prevented from creating a pull request if your branch can't be merged.

To resolve the conflict:

- Locally checkout the `main` branch.

- Pull the latest changes into `main` from the remote.

- Checkout your branch. (The one you wanted to merge.)

- Merge `main` into your branch.

- Resolve the conflicts using your editor or merge tool.

- Commit your changes to your branch.

- Push your branch to the remote.

- Attempt to create the pull request again.

## Source & Additional Links

[https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View](https://learn.rrc.ca/d2l/le/content/645955/viewContent/10531991/View).

[About Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).