# Astro Escape

An endless runner for Android built with Unity. Run, jump and dodge spikes, saws and falling rocks, collect coins, grab shields, and unlock new character skins and backgrounds.

> Play Store name: **Impostor Run** · Package: `com.rmbgamingcompany.ImpostorRun`

## Features

- One-touch endless running and jumping
- Moving hazards: sliding spike blocks, rolling saws, falling rocks, plus obstacles unique to each theme
- Shield pickup that absorbs one hit
- Coin arcs over obstacles
- Unlockable character skins and backgrounds
- Share your score with your own character skin
- Rewarded and interstitial ads (Google AdMob)
- In-app purchases: Remove Ads and coin packs (Unity IAP)
- Scales to phones and tablets, landscape orientation

## Requirements

- Unity **6000.3.28f1** (Unity 6.3 LTS) with Android Build Support (SDK, NDK, OpenJDK)
- Android minimum API level 25, target API level 36
- IL2CPP scripting backend

## Getting started

1. Clone the repository.
2. Open the folder in Unity Hub with the version above.
3. Open the main scene in `Assets/Scenes` and press Play.

## Building

Use the menu **Tools > Build**:

- **Test APK** builds an APK for testing.
- **Test APK and install** builds and installs it on a connected phone.
- **Release bundle (.aab)** builds the file for Google Play. Raise **Bundle Version Code** in Player Settings before every upload.

Keystore files are not stored in the repository. Keep your own keystore and passwords safe and out of Git.

## Monetization setup

- **AdMob:** the app ID is set in `Assets/GoogleMobileAds/Resources/GoogleMobileAdsSettings.asset`. Test ads are used in the editor and development builds; live ads in release builds. Do not click your own live ads.
- **In-app products** must exist in Play Console with these IDs:
  - `remove_ads` (non-consumable)
  - `coins_1000`, `coins_3000`, `coins_8000` (consumable)

## Project layout

| Folder | Contents |
| --- | --- |
| `Assets/Script` | Game code (player, enemies, hazards, pickups, ads, purchases, tutorial, share) |
| `Assets/Editor` | Build menu and editor tools |
| `Assets/Resources` | Runtime-loaded art such as the coin frames |
| `Assets/Plugins/Android` | Android libraries; some old androidx files are disabled to avoid duplicate-class build errors |
| `StoreAssets` | Play Store icon, feature graphic and screenshots |
| `docs` | Privacy policy page |

## Privacy

See [docs/privacy.html](docs/privacy.html).

## License

All rights reserved. Add a license here if you decide to open source the project.
