# GitHub Star Watching

## The value of watching random repos

> Open source tip: you’ll learn A LOT from taking a single project you actively use, “watching” it on GitHub and reading every issue and PR.
>
> -[Dan Abramov](https://twitter.com/dan_abramov/status/819555257055322112)

[How to be an open source gardener](https://steveklabnik.com/writing/how-to-be-an-open-source-gardener)

## Converting stars to watching
We do NOT want to watch public GitHub repos (very spammy) on our work/personal accounts (important notifications). Either we want a burner account and an e-mail filter, or an index on our local filesystem.

* For the burner account method: I have a script here that syncs `GITHUB_API_KEY_1`'s stars with `GITHUB_API_KEY_2`'s watch: https://github.com/llllvvuu/contributor-tools. I get around 10000 e-mails a day from this. It's essential to have the following settings in Gmail (TODO: experiment with other e-mail clients):
  - Compact mode
  - Keyboard shortcuts enabled
  - Auto-advance enabled
  - "Mark as important" seems to be Gmail's main inbox prioritization feature. TBD how well it actually works...
  - In order to not mess up the threading later, I use archive (e) or mute (m) instead of delete (#). I also auto-delete after 30 days: https://gist.github.com/jamesramsay/9298cf3f4ac584a3dc05?permalink_comment_id=4482003#gistcomment-4482003
  - https://ben.balter.com/2020/08/25/how-i-manage-github-notifications/
* TODO For the local filesystem method: create an indexer that keeps local database updated with issues from starred repos. Early POC here (script, not indexer): https://github.com/llllvvuu/contributor-tools

## Finding things to star
GitHub's new For You (Beta) is a lot better than their Explore page. It has a filter where you can remove "Announcements" and "Releases" since those can overwhelm the feed.

For it to be lively you need to be active in issues, PRs, discussions, stars, following people.

Following people is a great idea, and you can bootstrap it by following top contributors to the repositories you use, people you interact with in comment sections, etc.

## TODO
* ML ranking for watched GitHub issues
  * I assume such a thing doesn't exist yet because it's not relevant for work, where you have to read every notification anyway
  * For isolated personal setup, have to use something that's *not* based on some kind of collaborative filtering. Could be tricky.
