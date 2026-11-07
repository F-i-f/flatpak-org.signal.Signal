⚠️  Obsolete ⚠️
==============
org.signal.Signal Flatpak manifest simplified
==============================================

This was a fork of the [org.signal.Signal Flatpak manifest](https://github.com/flathub/org.signal.Signal).

# Update - 2026-11-07

Since [1513a6d8](https://github.com/flathub/org.signal.Signal/commit/1513a6d87dbb55df44bbb6bb80505d53d41c8fb7)
has been merged into the upstream manifest, this flatpak fork is no more
necessary, just add `SIGNAL_DISABLE_ENCRYPTION_WARNING=yes` to the
environment overrides to get the outcome this fork was providing.

This flatpak fork is not maintained anymore.

# Old fork information

As packaged in flathub, Signal prompts the user:
- to accept that the database is unencrypted.

There is no way for an administrator to prevent both dialogs to be shown.

This fork allows:
- to skip prompting the user to accept an unencrypted database if
  SIGNAL_PASSWORD_STORE is set:
  `flatpak override org.signal.Signal --env SIGNAL_PASSWORD_STORE=basic`

[Upstream README.md](README-upstream.md)
