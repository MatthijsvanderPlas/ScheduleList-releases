# ScheduleList — releases

Update feed for [ScheduleList](https://github.com/MatthijsvanderPlas/ScheduleList),
a macOS menubar app for tasks and meetings. **The source lives in that repo,
which is private — this one exists only to publish updates.**

[Sparkle](https://sparkle-project.org) inside the app polls the appcast here and
installs new versions on its own:

| | |
|---|---|
| Appcast | <https://matthijsvanderplas.github.io/ScheduleList-releases/appcast.xml> |
| Builds | the Releases tab — one tag per version |

Every build is signed with a Developer ID certificate, notarized by Apple, and
the appcast entry carries an EdDSA signature the app verifies before installing.
An update that fails any of those is refused.

Nothing here is edited by hand; `scripts/release.sh` in the source repo publishes
it.
