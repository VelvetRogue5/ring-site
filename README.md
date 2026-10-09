# Ring Bonbon Privacy Site

Static privacy site for Ring Bonbon (`ai.ringbonbon.game`), adapted from the structure of the Hanabi privacy page and styled to match Ring Bonbon. The English policy covers the current iOS and Android project configuration. The contact email is carried over from the reference site: `velvet_rogue_5@proton.me`.

## Pages

- `privacy.html`: privacy policy.
- `index.html`: redirects to the policy.
- `assets/`: local stylesheet and the current game icon. No third-party fonts, scripts, analytics, or cookies are added.

## Publish

In GitHub repository Settings → Pages, select Deploy from a branch, branch `main`, folder `/ (root)`.
Expected policy URL after Pages deployment: https://velvetrogue5.github.io/ring-site/privacy.html
Pushing the repository alone does not guarantee Pages has been enabled or deployed.

## Policy basis

Reviewed on October 9, 2026 against the Ring Bonbon Unity project at commit `81ccb0c`:

- `RingGameController.cs`: local PlayerPrefs level progress and coin balance.
- `SoundBank.cs`: local sound and vibration preferences.
- `RingGameController.Navigation.cs`: reads existing cosmetic inventory preferences; shop is not currently exposed.
- `Packages/manifest.json` and Assets: no integrated advertising, attribution, Firebase, or other analytics SDK found.
- `ProjectSettings/UnityConnectSettings.asset`: Unity services, analytics, ads, and cloud diagnostics disabled.
- No runtime network request, account, cloud-save, or purchase integration found in game scripts.

The policy intentionally does not copy Hanabi's advertising, Firebase, AppsFlyer, Meta, remote-level-download, or tracking clauses. Re-audit the final release build and update the policy and store privacy declarations before enabling such services. This is a description of the reviewed implementation, not a legal-compliance certification.
