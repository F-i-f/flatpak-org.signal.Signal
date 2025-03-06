org.signal.Signal Flatpak manifest simplified
==============================================

This is a fork of the [org.signal.Signal Flatpak manifest](https://github.com/flathub/org.signal.Signal).

As packaged in flathub, Signal prompts the user:
- to accept that the database is unencrypted.

There is no way for an administrator to prevent both dialogs to be shown.

This fork allows:
- to skip prompting the user to accept an unencrypted database if
  SIGNAL_PASSWORD_STORE is set:
  `flatpak override org.signal.Signal --env SIGNAL_PASSWORD_STORE=basic`

[Upstream README.md](README-upstream.md)
