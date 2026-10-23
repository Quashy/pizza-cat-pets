<p align="center"><a href="README.md">中文</a> | <strong>English</strong></p>

<p align="center">
  <img src="previews/pizza-pixel.png" alt="Pizza, a pixel cat in a cherry dress" width="256">
</p>

<h1 align="center">Pizza</h1>

<p align="center">Your pet. Your tiny on-screen supervisor.</p>

Wish your pet could keep you company at your desk? Turn a few photos into a realistic or pixel companion for coding sessions, homework, and well-earned breaks. No pet of your own? Pizza is ready to move in.

<p align="center">
  <a href="#create">Make your own</a> ·
  <a href="#install">Get Pizza</a> ·
  <a href="#preview">Preview both</a>
</p>

<p align="center">
  <img src="previews/pizza-photo-to-pet-comparison.png" alt="AI-assisted reference, realistic Pizza and 16-bit Pixel Pizza comparison" width="1000">
</p>

**Reference (AI-assisted cutout and completion)** · [View reference](previews/pizza-reference-ai-assisted.png)

The reference photo uses AI-assisted background removal and completion of obscured details. Explore both character styles and their animation previews below.

<a id="preview"></a>

## Two looks, one Pizza

| Original | Pixel |
| :---: | :---: |
| <img src="previews/pizza-original.png" alt="Realistic Pizza" width="192"> | <img src="previews/pizza-pixel.png" alt="16-bit Pixel Pizza" width="192"> |
| Realistic fur, cherry dress | 16-bit style, 128×128 logical canvas |
| <img src="previews/pizza-original.gif" alt="Original Pizza animation preview" width="192"> | <img src="previews/pizza-pixel.gif" alt="Pixel Pizza animation preview" width="192"> |
| [Sprite sheet](pets/original/spritesheet.png) | [Sprite sheet](pets/pixel/spritesheet.png) · [Native portrait](previews/pizza-pixel-native.png) |

<a id="create"></a>

## Have a pet of your own?

**Your photos → realistic and pixel characters → an animated desktop companion**

Copy the complete prompt below, or open the [creation prompt file](prompts/create-your-pet.md#english), and attach a few photos you have permission to use. Your AI will create **a realistic version and a 16-bit pixel version on a 128×128 logical canvas**. Approve the main looks, review the animation, then install and switch using your app's available capabilities.

### Copy to your AI

```text
Create two separate ChatGPT / Codex virtual pets from a few pet photos that I provide or explicitly identify and have permission to use: one realistic version and one 16-bit pixel version on a 128×128 logical canvas. Reference project: https://github.com/Quashy/pizza-cat-pets . Use it as a reference for the two styles and final format; the character must be my pet. Do not install Pizza and present it as my own pet.

Before starting, confirm the pet's name; facial shape, fur color, markings, and other traits to preserve; clothing to keep or add; the detailed visual preferences for each version. The required output is already realistic plus 16-bit pixel art on a 128×128 logical canvas; do not substitute another bit depth or canvas. Ask only for necessary additional angles. Do not use photos of unknown origin or publish my source photos or personal information.

If the photos contain occlusions or missing details, reasonably complete the body and clothing while preserving key identity traits. Ask me about uncertain defining traits first, and distinguish AI-completed details from what is actually visible in the photos; do not present completed details as if they were present in the original photos.

Generate one clear main-look preview first, preserving identity, proportions, colors, and clothing. Show it at the intended display size for my approval before generating all animations. Approve the realistic and pixel main looks separately and keep them as separate versions throughout.

After approval, verify the target app's Pets v2 support. Deliver transparent 1536×2288 PNGs with 8 columns, 11 rows, 192×208 cells, 9 states, and 16 look directions. If the target app cannot use them, explain that limitation rather than silently downgrading. Create the idle, left/right movement, wave, jump, error, waiting, working, and review animations, plus supported look directions. Keep identity, colors, scale, registration, and anatomy consistent. A jump should visibly leave the ground; movement and gaze must face the correct directions. For pixel art, keep crisp edges and the agreed logical canvas; do not confuse that canvas with the final install sheet's dimensions.

Review each animation for pink background spill, exposure or color flicker, sudden tail or head jumps, clipping, missing frames, reversed directions, and broken motion. Keep transparency clean. Repair the affected animation while preserving approved work.

Show motion previews of the main actions and look directions for my approval before installation. Deliver the final install sheet, a viewable portrait, and animation previews. Do not publish my photos or personal details by default.

Before installing, detect my actual app, version, tools, and local access. Use a verified custom-pet import method. Do not claim ordinary ChatGPT chats can always install pets or modify a local computer, and do not invent pet directories or configuration. If image generation, validation, file access, or installation is unavailable, explain the exact stopping point, completed work, and what I need to provide or do manually. Never pretend it succeeded.

Save an independent pet. Name and record the realistic and pixel versions separately with their actual stable IDs or verified local IDs. Do not overwrite, delete, or replace existing pets. Let me choose the active version, switch only to the one I request, verify the result, and explain how to switch later.
```

<a id="install"></a>

## Want Pizza instead?

Copy the complete prompt below, or open the [installation prompt file](prompts/install.md#english), and send it to your AI. It will check your app's capabilities, install **Pizza Original** and **Pizza Pixel** separately, and activate the realistic Original by default while preserving existing pets.

Then say **“Switch to Pizza Pixel”** or **“Switch to Pizza Original.”** Both prompts include the repository URL and work as standalone requests.

### Copy to your AI

```text
Install both Pizza versions from https://github.com/Quashy/pizza-cat-pets into my actual ChatGPT / Codex environment. Keep both and activate the realistic Pizza Original by default so I can switch later.

Source and files:
- Repository: https://github.com/Quashy/pizza-cat-pets . Fetch the files from this repository; do not guess other URLs or use another account's private assets.
- Original: https://raw.githubusercontent.com/Quashy/pizza-cat-pets/main/pets/original/spritesheet.png ; display name Pizza Original.
- Pixel: https://raw.githubusercontent.com/Quashy/pizza-cat-pets/main/pets/pixel/spritesheet.png ; display name Pizza Pixel.
- Both are transparent PNGs, Pets v2, 1536×2288, 8 columns × 11 rows, with 192×208 cells. The first nine rows contain 6/8/8/4/5/8/6/6/6 frames; the last two contain 16 look directions. Portrait previews and GIFs are not install files.

1. Detect the actual app, version, OS, available tools, and current official installation guidance first. Distinguish desktop, web, Codex CLI, IDE, and dot. Use only a verified v2-capable route. Do not assume a normal chat can access my computer, or invent directories, configuration fields, tool arguments, or success.
2. Fetch the two PNGs from the confirmed repository. Check their type, dimensions, transparency, and integrity without altering the originals or replacing existing pets. If you cannot download or access files, tell me exactly which files to download or attach.
3. Choose one route based on actual capabilities:
   - If Pets creation tools are available, list existing pets first to avoid duplicates. For each PNG, call validate_pet_spritesheet; continue only if valid=true. Call prepare_pet_upload, then create_pet using the actual returned upload_session_id. Complete and verify the upload as required by the current tools. Record the stable pet.id returned by create_pet. A temporary URL, upload session, or repository filename is not a pet ID. Verify each creation and its list entry. If only one succeeds, preserve it, check the uncertain result before retrying, and avoid duplicates.
   - If the desktop app supports the official pet install flow, build a separate codex://pets/install link for each version. Use its display name as name, the PNG's public raw HTTPS URL at the repository's actual branch or commit as imageUrl, and spriteVersionNumber=2. URL-encode parameters correctly. Verify support first, then have me open the links and complete installation in the app. Reference: https://learn.chatgpt.com/docs/reference/commands#pets . Opening the flow alone does not prove installation; verify the result.
   - If the app explicitly supports local folder installation, read its current official documentation or installed official pet installation skill to verify the real directory and configuration format. Install with two separate, non-conflicting local IDs/directories. If needed, convert only a copy losslessly and verify it. Do not reuse another version's schema, change global settings without authorization, overwrite a directory, or confuse a copied file with an active pet.
4. After installation, record each version's display name, actual stable ID (or verified local ID), source file, and install location. Save that mapping appropriately in my own environment for later switching; never write my information into the public repository. After installing both, activate the realistic Pizza Original by default, unless I explicitly choose a different version in this request.
5. Switch only to the version I requested, resolving its actual ID on my account/device first; clarify duplicate names. In a supported ChatGPT Pets environment, use select_pet and verify active_pet_id. For a dot's appearance, use the actually available cloud_threads.select_orbit_pet; a global selection does not prove the dot changed. In the local desktop app, refresh and select in Settings > Pets. Only use /pets in a supported graphics terminal after verifying that the actual Codex CLI loader accepts these v2 files. The checked public CLI source still accepts only v1 and cannot directly use these v2 sheets. Keep the other version installed. Never reuse the publisher's account-specific pet IDs.
6. If no verified installation or switching capability is available, stop that step and explain the limitation, completed work, and exact action I must take. The documented ordinary web upload currently specifies v1 (1536×1872); do not claim these v2 files are compatible, trim their look directions, or silently downgrade them. The IDE extension has no pet picker. Codex CLI display also depends on terminal graphics support, so visibility is not guaranteed in every terminal.
Finish with a short report of each version's installation result, the active version, stable IDs, and how to switch later.
```

## Compatibility

- Both are transparent Pets v2 PNGs: 1536×2288, 8 columns × 11 rows, 192×208 cells, 9 states and 16 look directions. 128×128 describes the pixel artwork, not the install file.
- Requires a v2-capable desktop pet install flow or Pets tools. An ordinary ChatGPT chat may not install pets or access your computer. Local folder installation requires verification of the actual version and format.
- The documented ordinary web upload and the checked Codex CLI loader currently require v1 (1536×1872) and cannot directly use these v2 files. CLI display also depends on terminal graphics support; the IDE extension has no pet picker.

[Official Pets guide](https://learn.chatgpt.com/docs/pets) · [Desktop install flow](https://learn.chatgpt.com/docs/reference/commands#pets) · [Checked CLI loader](https://github.com/openai/codex/blob/398500106707f0a3217c7cf83edc2bf226cc342f/codex-rs/tui/src/pets/model.rs#L314)
