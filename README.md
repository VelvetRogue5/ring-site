# Ring Bonbon Privacy Site

Static privacy site for Ring Bonbon (`ai.ringbonbon.game`), adapted from the structure of the Hanabi privacy page and styled to match Ring Bonbon. The English policy covers iOS and Android, including the planned advertising, Firebase, Meta (Facebook) SDK, and AppsFlyer integrations. The contact email is carried over from the reference site: `velvet_rogue_5@proton.me`.

## Pages

- `privacy.html`: privacy policy.
- `marketing.html`: English store listing drafts and release verification notes for iOS and Android.
- `terms-of-use.html`: terms of use, referring to Apple's standard EULA for App Store distribution rather than declaring a custom EULA.
- `support/index.html`: public technical support and gameplay help.
- `index.html`: redirects to the policy.
- `assets/`: local stylesheet and the current game icon. No third-party fonts, scripts, analytics, or cookies are added.

## Publish

In GitHub repository Settings → Pages, select Deploy from a branch, branch `main`, folder `/ (root)`.
Expected policy URL after Pages deployment: https://velvetrogue5.github.io/ring-site/privacy.html
Support URL: https://velvetrogue5.github.io/ring-site/support/
Marketing URL: https://velvetrogue5.github.io/ring-site/marketing.html
Terms URL: https://velvetrogue5.github.io/ring-site/terms-of-use.html
Pushing the repository alone does not guarantee Pages has been enabled or deployed.

## Policy basis

Updated on October 12, 2026 ahead of the advertising, Firebase, Meta (Facebook) SDK, and AppsFlyer integrations requested by the project owner. The October 9 review of the Unity project at commit `81ccb0c` established local PlayerPrefs saves and no account or in-app purchases; it predates the SDK integration work.

The policy now covers conditional SDK data collection, purposes, sharing, advertising identifiers, consent and system controls, retention, privacy requests, and children's privacy. Advertising channels follow the project owner's reference at `/Users/sanmu/Desktop/paperboom-site/`: AppLovin MAX mediation; AppLovin, Unity Ads, Vungle (Liftoff), Mintegral, Pangle (ByteDance), BidMachine, and Bigo Ads on both platforms, plus Google AdMob and DT Exchange on iOS. They are disclosed as planned integrations, with actual availability dependent on the release configuration.

Provider references use Firebase's privacy documentation, Meta's privacy policy, and AppsFlyer's Services Privacy Policy.

Before release, verify enabled Firebase products, Meta and AppsFlyer events and identifier settings, the final ad network and mediation partners, consent behavior, age restrictions, and retention against the release build. Confirm the listed advertising partners against the final platform builds, and align App Store privacy and Google Play Data safety declarations with actual behavior. Updating this page does not configure SDK consent or certify legal compliance.
