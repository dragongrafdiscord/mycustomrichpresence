# Preset Overhaul Audit

Generated: 2026-08-27

## Result

- Total presets: **57**
- Personal: **10**
- Requested: **40**
- General: **5**
- Community: **2**

## Global changes

- Removed the old `mypresets/mightdelete/` structure; Demonic remains a normal preset.
- Removed the Application ID from every preset, including the two existing community presets.
- Normalized presets to the current field roster (`Type`, `Display`, `Name`, URL fields, end timestamp fields, etc.).
- Preserved existing text, party settings, timestamps, image URLs and intentional joke buttons wherever the current file was available.
- Restored versioned duplicates instead of deleting them (`Sleeping v1/v2`, `YouTube v1/v2`, `Netflix v1/v2`, `Counter-Strike 2 v1/v2/v3`).
- Added local preview PNGs under `assets/previews/` for every preset.
- Added `presets.json` as the machine-readable roster.
- Imported no new community presets from the Discord channel.

## Exact/recovered files

- **Arch Linux (Tofix)** — current-repo (`Arch_by_Tofix.rs.crp`)
- **ARK 2 (Kamy)** — current-repo (`ark2.crp`)
- **Beast Boy** — current-repo (`beastboy.crp`)
- **Blender** — current-repo (`Blender.crp`)
- **Call of Duty Black Ops 2** — current-repo (`Call of Duty Black Ops 2.crp`)
- **Counter-Strike 2 v3** — recent-request (`Counter-Strike 2 v3.crp`)
- **Crazy** — current-repo (`crazy.crp`)
- **DDLC Larping** — recent-request (`DDLC Larping.crp`)
- **Dead by Daylight** — recent-request (`Dead by Daylight.crp`)
- **Demonic** — current-repo (`mightdelete/demonic.crp`)
- **Dragon** — current-repo (`Dragon.crp`)
- **Editing Videos** — current-repo (`editing.crp`)
- **Fortnite** — recent-request (`Fortnite.crp`)
- **Grand Theft Auto VI** — recent-request (`Grand Theft Auto VI.crp`)
- **Growtopia** — current-repo (`Growtopia.crp`)
- **Halloween** — current-repo (`Halloween.crp`)
- **Kali Linux** — recent-request (`Kali Linux.crp`)
- **Netflix v2** — current-repo (`netflix.crp`)
- **Pornhub** — current-repo (`Pornhub.crp`)
- **Python DE** — current-repo (`python preset DE.crp`)
- **Red Bull** — recent-request (`Red Bull.crp`)
- **Sleeping v1** — older-repo-snapshot (`sleepingoriginal.crp`)
- **Sleeping v2** — older-repo-snapshot (`sleeping.crp`)
- **That Time I Got Reincarnated as a Slime** — current-repo (`That Time I Got Reincarnated as a Slime.crp`)
- **THE BIRD IS THE WORD** — current-repo (`THE BIRD IS THE WORD.crp`)
- **Visual Studio** — current-repo (`Visual_Studio.crp`)
- **YouTube v1** — current-repo (`youtube.crp`)
- **YouTube v2** — current-repo (`youtube_v2.crp`)

## Reconstructed presets

These existed in the Discord preset history (or were explicitly requested for the new Personal roster), but an original local `.crp` attachment was not present in the supplied repo snapshots. They were rebuilt conservatively instead of being dropped.

- **08.12 Birthday** — reconstructed-from-discord-post — Discord message `1048647683184791743`
- **Counter-Strike 2 v1** — reconstructed-from-discord-post — Discord message `1090401833530429470`
- **Counter-Strike 2 v2** — reconstructed-from-discord-post — Discord message `1090402246849728633`
- **Cyberpunk 2077** — reconstructed-from-discord-post — Discord message `1260082823209947197`
- **Cyberpunk Edgerunners** — reconstructed-from-discord-post — Discord message `1260080541487599657`
- **Epic Games** — reconstructed-from-discord-post — Discord message `1119834790057738342`
- **Equalizer APO** — reconstructed-from-discord-post — Discord message `1093612467432726630`
- **Free Fire** — reconstructed-from-discord-post — Discord message `1119831975713320970`
- **Genshin Impact** — reconstructed-from-discord-post — Discord message `1048649487293358170`
- **GitHub** — recreated-personal
- **GTA Santos** — reconstructed-from-discord-post — Discord message `1115091686096388146`
- **Half-Life 3** — reconstructed-from-discord-post — Discord message `1133607717966204939`
- **LEGO Batman** — reconstructed-from-discord-post — Discord message `1135406808178102433`
- **Mommy ASMR Simulator** — reconstructed-from-discord-post — Discord message `1309415117347094588`
- **Netflix v1** — reconstructed-from-discord-post — Discord message `1044078048506560553`
- **OnlyFans** — reconstructed-from-discord-post — Discord message `1255096744480477236`
- **PUBG** — reconstructed-from-discord-post — Discord message `1115092509794779176`
- **Python** — reconstructed-from-discord-post — Discord message `1109269963157540915`
- **Relaxing** — reconstructed-from-discord-post — Discord message `1135403639402401902`
- **Resident Evil 4 Remake** — reconstructed-from-discord-post — Discord message `1118169321844260864`
- **Streaming on Twitch** — recreated-personal
- **Trainz Railroad Simulator 2019** — reconstructed-from-discord-post — Discord message `1094667028708720771`
- **Valorant** — reconstructed-from-discord-post — Discord message `1052259683802554420`
- **Vegas Pro** — reconstructed-from-discord-post — Discord message `1256985658887639060`
- **Visual Studio Code** — reconstructed-from-discord-post — Discord message `1094669254533582981`
- **VRChat** — reconstructed-from-discord-post — Discord message `1254284363550691339`
- **Watch Dogs 2** — reconstructed-from-discord-post — Discord message `1255982276576022528`
- **Xanax** — reconstructed-from-discord-post — Discord message `1135695939441528872`
- **Zelda: Tears of the Kingdom** — reconstructed-from-discord-post — Discord message `1115093080945721375`

## Requester IDs still unknown

- **Epic Games** — requester: Deleted User
- **Equalizer APO** — requester: Deleted User
- **Free Fire** — requester: Deleted User
- **GTA Santos** — requester: Deleted User
- **Grand Theft Auto VI** — requester: Remi
- **Halloween** — requester: Deleted User
- **Kali Linux** — requester: unknown
- **Mommy ASMR Simulator** — requester: Deleted User
- **Pornhub** — requester: Unknown
- **Python** — requester: Deleted User
- **Resident Evil 4 Remake** — requester: Deleted User
- **Visual Studio** — requester: Deleted User

## Preview handling

- Local previews are regenerated from the modernized preset fields so every README entry has a stable in-repo image.
- `presets.json` retains `originalPreviewUrl` when the old README or Discord export exposed one.
- Signed Discord CDN URLs in old HTML exports are historical references and may no longer download. They were not silently replaced with unrelated artwork.

## Presence artwork

- Existing direct `LargeKey` / `SmallKey` image URLs were preserved where the original/current preset was available.
- Reconstructed historical presets do not invent a replacement image when the original artwork could not be recovered.
- `assets/presence/` is reserved for mirroring those images later if desired.
