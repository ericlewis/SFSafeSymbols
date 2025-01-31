# Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/piknotech/SFSafeSymbols. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.

## Getting Started

In order to generate the **Xcode project** to develop within, run this command:

```
swift package generate-xcodeproj
```

### Commit Messages

Please try to follow the same syntax and semantic in your **commit messages** (see rationale [here](http://chris.beams.io/posts/git-commit/)).

### Tracking Changes

When issuing a pull request, please add a summary of your changes to the `CHANGELOG.md` file and credit yourself as the author.

## Releasing

To release a new version, do the following things:

1. Bump the build num in the `SFSafeSymbols.podspec` and at all places in the `README.md` (Version Badge, Version Badge Alt Text, Installation Instructions).
2. Update the `CHANGELOG.md` file by changing the *Unreleased* title to the version num and the release date. Then add a new *Unreleased* Section on top, maintaining the 3 existing subsections (Added, Changed, Fixed).
3. Release on GitHub and copy the changelog contents for this version into the release notes on GitHub.
4. Publish on CocoaPods using `pod trunk push SFSafeSymbols.podspec`.
