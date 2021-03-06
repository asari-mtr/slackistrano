# Slackistrano Change Log

3.1.1
-----

- Allow easily disabling Slackistrano by setting :slackistrano to false [#67]

3.1.0
-----

- An entirely new way of customizing the messages sent to Slack. See the README for details.

3.0.0
-----

- Require version 3.5.0 of Capistrano and utilize it's new dry-run functionality.

2.0.1
-----

- Internal code refactoring. No public facing changes.

2.0.0
-----

- **BREAKING:** You must now `require 'slackistrano/capistrano'` in your Capfile.
  Previously it was just `require 'slackistrano'`. It is also no longer necessary
  to add `require: false` in your Gemfile, but it won't hurt to leave it.

1.1.0
-----

- Honor Capistrano's `--dry-run` [#33]
- Better error reporting if Slack API returns failure [#40]
- Allow posting to multiple channels by setting `:slack_channel` to an array [#37]


1.0.0
-----

- **BREAKING:** Renamed all `***_starting` settings to `***_updating`
- **BREAKING:** Renamed all `***_finished` settings to `***_updated`
- Added rollback options `***_reverting` and `***_reverted` [#19, #31]

