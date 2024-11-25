org.signal.Signal Flatpak manifest simplified
==============================================

This is a fork of the [com.signal.Signal Flatpak manifest](https://github.com/flathub/com.signal.Signal).

As packaged in flathub, Signal prompts the user:
- to accept that the database is unencrypted,
- to accept host filesystem access.

There is no way for an administrator to prevent both dialogs to be shown.

This fork allows:
- to skip prompting the user to accept an unencrypted database if
  SIGNAL_PASSWORD_STORE is set:
  `flatpak override org.signal.Signal --env SIGNAL_PASSWORD_STORE=basic`
- to skip prompting the user to accept host file system access if
  SIGNAL_HOST_FILESYSTEM_OK is set to yes:
  `flatpak override org.signal.Signal --env SIGNAL_HOST_FILESYSTEM_OK=yes`

[Upstream README.md](README-upstream.md)
