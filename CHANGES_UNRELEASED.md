**See [the release process docs](docs/howtos/cut-a-new-release.md) for the steps to take when cutting a new release.**

# Unreleased Changes

[Full Changelog](https://github.com/mozilla/application-services/compare/v0.48.3...master)

## FxA Client

### What's New

- `FirefoxAccount` is now deprecated
- Introducing `FxAccountManager` which provides a higher-level interface to Firefox Accounts. Among other things, this class handles (and can recover from) authentication errors, exposes device-related account methods, handles its own keychain storage and fires observer notifications for important account events.

### Breaking changes

- `FirefoxAccount.fromJSON(json: String)` has been replaced by the `FirefoxAccount(fromJsonState: String)` constructor.

