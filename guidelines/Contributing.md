## Getting started

There are 3 core contribution pillars:
1. **Goal** – a business aim
1. **Problem** – an issue that is on our way to achieving the Goal
1. **Solution** –  the actual deliverable which resolves the problem

> [!NOTE]
> In this guide you will get an overview of the contribution workflow: from finding a Goal, identifying a Problem, and the process of delivering your solutions.

### Goal

As soon as you get involved, you must understand the goal you are working on by

1. investigating the conversations and related documents
1. understanding how things are already moving towards achieving the goal 

It is crucial to understand the business context of the goal and how achieving the goal will impact the project.

> [!NOTE]
> A Goal is represented as a GitHub issue in the relevant repository and has the following naming pattern: `Goal: [statement]`.  

### Problem

Once the Goal is clear, you must identify what stops you from achieving it. Anything that is stopping you - is a “Problem”. A typical question to ask is: "Why is this Goal not achieved and what is the Problem?" using the POV of the end user.

Sometimes, a Goal already has a few identified problems, but not always.

> [!NOTE]
> Once a Problem is identified, we report it as a [GitHub Issue](https://docs.github.com/en/issues) with the following naming pattern: `Problem: [statement]`.  
> We’re counting on our contributors to identify problems. Keep a Problem name short (under 65 chars) and crystal clear.

Make sure each Problem issue is interlinked with it's Goal issue:
- add a Problem issue link into the Goal description
- add a Goal issue link to the Problem description

It's essential to maintain clear links between Goals and related Problem issues. This helps everyone stay informed and team members can easily track progress and understand the context.

### Solution

The third pillar of successful contribution is the Solution.

Different problems may require different sets of skills.  
Whether it’s code, design, or marketing material, we expect a lean and clean solution from the contributor.

> [!NOTE]
> Solution is presented in GitHub as [Pull Requests (PR)](https://docs.github.com/en/pull-requests) in compliance with [PR Requirements](#pr-requirements).

# PR Requirements
All PRs, whether for source code, design, or copy changes, must comply with our PR Requirements.


## Commit Signature Verification

For the security and integrity of our project, we require all contributors to sign their commits.  
For detailed instructions on why and how to sign your commits refer to [GitHub's documentation on commit signature verification](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification).

> [!Note]
> We recommend signing commits using an [SSH key](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification#ssh-commit-signature-verification). Ensure your Git version supports SSH signature verification (Git 2.34 or later).

## Scoping

When planning the scope of work, make sure you [keep PRs small](https://artsy.github.io/blog/2021/03/09/strategies-for-small-focused-pull-requests/). You must be able to complete your PR within 3-4 hours.  
If the solution requires more time, then decompose it into smaller independent PRs. In case your smaller PRs can't be used on production, use feature flags.


## Naming

We are using commits (PR names) to communicate the release log to all stakeholders, including non-technical ones.  
Thus, the names of the PRs must:
1. be oriented toward the end users
1. follow [Conventional Commits Guidelines](https://www.conventionalcommits.org)
2. be [clean and simple](https://pulsar.apache.org/contribute/develop-semantic-title/#how-to-write-good-pr-titles)

```
// Good examples:
 - feat(ui): play music
 - fix(sdk): mute sound
 - test(api): open door

// Bad examples:
 - create a player
 - fix: add a file to mute sound
 - feat: modified door function
```

#### Code Quality and Reviews

Aim for solutions that work correctly 99.9% of the time. Be independent and thorough in your QA - reviewers are not QA team members but are there for a final safety check. We expect contributors to deliver bug-free software, understanding that perfection is an ideal. Stand firm in your solutions and avoid unnecessary revisions based on subjective feedback.