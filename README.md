<p align="center">
  <img src="previews/pizza-pixel.png" alt="披萨 Pizza — a golden cat in a cherry dress, in pixel art" width="256">
</p>

<h1 align="center">披萨 · Pizza</h1>

<p align="center">让你家的毛孩子来屏幕里监工。<br>Your pet. Your tiny on-screen supervisor.</p>

想把你家的毛孩子搬进屏幕，当你的专属小监工吗？用几张照片，把它变成写实或像素模样，陪你写代码、赶作业、摸会儿鱼。没有宠物？先领一只披萨回去。

Wish your pet could keep you company at your desk? Turn a few photos into a realistic or pixel companion for coding sessions, homework, and well-earned breaks. No pet of your own? Pizza is ready to move in.

<p align="center">
  <a href="#create">用自己的宠物制作 · Make your own</a> ·
  <a href="#install">直接使用披萨 · Get Pizza</a> ·
  <a href="#preview">查看两版 · Preview</a>
</p>

<p align="center">
  <img src="previews/pizza-photo-to-pet-comparison.png" alt="AI辅助参考照片、写实披萨与16-bit像素披萨对照 / AI-assisted reference, realistic Pizza and 16-bit Pixel Pizza comparison" width="1000">
</p>

**参考照片（AI 去背景及补全）/ Reference (AI-assisted cutout and completion)** · [查看参考图 / View reference](previews/pizza-reference-ai-assisted.png)

参考照片已通过AI移除背景并补全遮挡细节。下方展示两版形象与动作预览。

The reference photo uses AI-assisted background removal and completion of obscured details. Explore both character styles and their animation previews below.

<a id="preview"></a>
## 两种模样，同一个披萨 / Two looks, one Pizza

| 原版 / Original | 像素版 / Pixel |
| :---: | :---: |
| <img src="previews/pizza-original.png" alt="写实版披萨 / Realistic Pizza" width="192"> | <img src="previews/pizza-pixel.png" alt="16-bit像素版披萨 / 16-bit Pixel Pizza" width="192"> |
| 写实毛绒质感，樱桃裙 / Realistic fur, cherry dress | 16-bit 风格，128×128 逻辑画布 / 16-bit style, 128×128 logical canvas |
| <img src="previews/pizza-original.gif" alt="原版披萨动作预览 / Original Pizza animation" width="192"> | <img src="previews/pizza-pixel.gif" alt="像素版披萨动作预览 / Pixel Pizza animation" width="192"> |
| [宠物 PNG / Sprite sheet](pets/original/spritesheet.png) | [宠物 PNG / Sprite sheet](pets/pixel/spritesheet.png) · [原生主图 / Native portrait](previews/pizza-pixel-native.png) |

<a id="create"></a>
## 有自己的宠物？/ Have a pet of your own?

**你的照片 → 写实与像素形象 → 会动的桌面陪伴**<br>
**Your photos → realistic and pixel characters → an animated desktop companion**

复制 [创建提示词](prompts/create-your-pet.md)，附上少量你有权使用的照片，让 AI 制作 **写实版＋16-bit、128×128 逻辑画布像素版**。先确认主形象，再看动作预览，最后按应用实际能力安装和切换。

Copy the [creation prompt](prompts/create-your-pet.md) and attach a few photos you have permission to use. Your AI will create **a realistic version and a 16-bit pixel version on a 128×128 logical canvas**. Approve the main looks, review the animation, then install and switch using your app's available capabilities.

### 中文提示词

```text
请基于我提供或明确指定且有权使用的少量宠物照片，帮我制作 ChatGPT / Codex 虚拟宠物，必须分别提供写实版和16-bit像素版，像素版使用128×128逻辑画布。参考项目：https://github.com/Quashy/pizza-cat-pets 。参考它的两种风格与成品规格，角色必须来自我的宠物，不要直接安装披萨来冒充我的宠物。

开始前先和我确认：宠物名字；必须保留的脸型、毛色、花纹和其他特征；是否保留或添加服装；两版的具体表现偏好。目标已确定为写实＋16-bit、128×128逻辑画布像素版，不改成其他位深或画布。照片不足时只索取必要角度，不使用不明来源的照片，不把原照片或个人信息公开。

照片有遮挡或细节缺失时，可以合理补全身体与服装，保持关键身份特征；不确定的关键特征先向我询问，并明确区分AI补全与照片中实际可见的细节，不要把补全内容说成原照片已有细节。

先生成一张清晰的主形象预览，保留宠物身份、比例、配色和服装细节，在实际显示尺寸下让我确认。确认前不要批量生成全部动作。分别确认写实版和像素版主形象，并始终保留为独立版本。

主形象确认后，核实目标应用对Pets v2的支持；目标成品为透明1536×2288 PNG、8列11行、192×208单元、9种状态和16个注视方向。目标应用不支持时明确告知，不静默降级。然后制作待机、左右移动、招手、跳跃、出错、等待、工作和查看等动作，以及应用支持的注视方向。全程保持身份、颜色、大小、画面位置和身体结构一致；跳跃应有真实离地，左右移动与注视方向必须正确。像素版保持清晰像素边缘和约定的逻辑画布，不把逻辑画布尺寸误当成最终安装图尺寸。

逐动作检查粉色背景溢色、帧间曝光或颜色闪烁、尾巴或头部突然跳变、裁切、缺帧、方向反转和动作不连贯。透明背景应干净。发现问题先修复对应动作，保留已经满意的部分。

完成后先给我看常用动作与方向变化的运动预览，让我确认实际播放效果，再安装。提供最终安装图、便于观看的主图和动作预览；默认不发布我的照片或任何个人资料。

安装前探测我当前应用、版本、真实工具与本地访问能力，使用已核实的自定义宠物导入方式。不要声称普通ChatGPT聊天都能安装或修改本地电脑，不要编造宠物目录或配置。若缺少图片生成、验证、文件访问或安装能力，明确说明停在哪一步、已完成什么、需要我提供什么或手动完成什么，不假装成功。

保存为独立宠物；写实版与像素版分别命名并记录实际稳定ID或经核实的本地ID，不覆盖、删除或替换已有宠物。让我选择当前启用的版本，并按我指定的版本切换，完成后核实结果，告诉我以后如何切换。
```

### English prompt

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
## 想直接使用披萨？/ Want Pizza instead?

复制 [安装提示词](prompts/install.md) 给你的 AI。它会检查应用能力，分别安装 **Pizza Original** 和 **Pizza Pixel**，并默认启用写实原版，保留已有宠物。

Copy the [installation prompt](prompts/install.md) to your AI. It will check your app's capabilities, install **Pizza Original** and **Pizza Pixel** separately, and activate the realistic Original by default while preserving existing pets.

之后说 **“切换到像素版披萨”** 或 **“切换到原版披萨”**。两份提示词都内含仓库链接，可独立复制分享。

Then say **“Switch to Pizza Pixel”** or **“Switch to Pizza Original.”** Both prompts include the repository URL and work as standalone requests.

### 中文提示词

```text
请把 https://github.com/Quashy/pizza-cat-pets 中的两版 Pizza / 披萨宠物安装到我实际使用的 ChatGPT / Codex 环境，保留两版，并默认激活写实原版 Pizza Original，之后可分别切换。

来源与文件：
- 仓库：https://github.com/Quashy/pizza-cat-pets 。从该仓库获取文件，不猜测其他链接或使用其他账户的私有资源。
- 原版：https://raw.githubusercontent.com/Quashy/pizza-cat-pets/main/pets/original/spritesheet.png ，显示名 Pizza Original（披萨·原版）。
- 像素版：https://raw.githubusercontent.com/Quashy/pizza-cat-pets/main/pets/pixel/spritesheet.png ，显示名 Pizza Pixel（披萨·像素版）。
- 两者均是透明 PNG、Pets v2、1536×2288、8列11行、192×208 单元。前9行动作帧数为6/8/8/4/5/8/6/6/6；最后2行是16个注视方向。预览图和GIF不是安装文件。

1. 先探测当前应用、版本、操作系统、实际可调用工具和当前官方安装说明。区分桌面应用、网页、Codex CLI、IDE 和 dot。只使用已确认支持 v2 的路径。不要假设普通聊天能访问我的电脑，不要编造安装目录、配置字段、工具参数或成功结果。
2. 从确认的仓库获取两张 PNG，检查文件类型、尺寸、透明背景及完整性，不修改原图或覆盖已有宠物。若没有下载或文件访问能力，告诉我需要下载/附上哪些文件。
3. 根据实际能力选择一种安装路径：
   - 如果当前环境提供 Pets 创建工具，先读取已有宠物列表，避免重复；分别对每张 PNG 执行 validate_pet_spritesheet，只有 valid=true 才调用 prepare_pet_upload，并用实际返回的 upload_session_id 调用 create_pet。按当前工具要求完成并核实上传，保存 create_pet 返回的稳定 pet.id。不要把临时链接、上传会话或本仓库的文件名当成 pet ID。逐一核实创建结果与列表；中途失败时保留已成功安装的一版，查明结果后再重试，避免重复创建。
   - 如果桌面应用提供官方宠物安装入口，可为两版分别构造 codex://pets/install 链接：name 为对应显示名；imageUrl 为该仓库实际分支或提交上 PNG 原始文件的公开 HTTPS 地址；spriteVersionNumber=2；各参数正确 URL 编码。先核实应用支持该入口，再让我打开并完成界面安装。官方入口参考：https://learn.chatgpt.com/docs/reference/commands#pets 。打开入口不等于安装完成，必须核实。
   - 如果应用明确支持本地目录安装，先读取当前应用的官方资料或已安装的官方宠物安装技能，核实真实目录和配置格式，再使用两个独立且不冲突的 ID/目录安装。必要时仅对副本做无损格式转换并复核。不要套用其他版本的配置，不要擅自修改全局设置、覆盖已有目录或将文件复制成功当作已启用。
4. 安装成功后，为我记录每版的显示名、实际稳定 ID（或已核实的本地 ID）、对应文件和安装位置；用当前环境适当的方式保存这份记录以便以后切换，不向公共仓库写入我的信息。两版都安装后默认激活写实原版 Pizza Original；若我在本次请求中明确另选了版本，按我指定的版本激活。
5. 切换必须按我指定的原版/像素版，先解析我自己账户或设备上的实际 ID，重名时确认。支持的 ChatGPT Pets 环境用 select_pet 并核实 active_pet_id；dot 形象选择使用实际可用的 cloud_threads.select_orbit_pet，不要把全局选择当成 dot 已切换。本地桌面应用在 Settings > Pets 刷新并选择。仅在已经确认当前 Codex CLI 读取器接受本仓库 v2 文件后，才在支持的图形终端中用 /pets 选择并核实；已核实的公开 CLI 源码仍只接受 v1，不能直接用这些 v2 文件。不删除另一版，也不使用发布者账户的 pet ID。
6. 如果没有已证实可用的安装/切换能力，停在该步骤，明确说明应用限制、已完成的部分、仍需我做的操作。普通网页上传的官方说明目前限定 v1（1536×1872），不能把本仓库 v2 文件谎称为兼容；不要裁掉方向帧或静默降级。IDE 扩展不提供宠物选择器。Codex CLI 的宠物显示还受终端图形支持影响，不能保证所有终端可见。
完成后简要汇报两版各自的安装结果、当前激活版本、稳定 ID 和以后切换的方法。
```

### English prompt

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

## 兼容性 / Compatibility

- 两版均为透明 Pets v2 PNG：1536×2288，8列×11行，192×208 单元，9种状态与16个注视方向。128×128 指像素创作画布，不是安装文件尺寸。<br>Both are transparent Pets v2 PNGs: 1536×2288, 8 columns × 11 rows, 192×208 cells, 9 states and 16 look directions. 128×128 describes the pixel artwork, not the install file.
- 需要支持 v2 的桌面宠物安装入口或 Pets 工具。普通 ChatGPT 对话不保证能安装或访问电脑；本地目录安装须核实实际版本与格式。<br>Requires a v2-capable desktop pet install flow or Pets tools. An ordinary ChatGPT chat may not install pets or access your computer. Local folder installation requires verification of the actual version and format.
- 网页普通上传说明及核实到的 Codex CLI 读取器目前仍限定 v1（1536×1872），不能直接使用这里的 v2 文件。CLI 显示还取决于终端图形支持；IDE 扩展没有宠物选择器。<br>The documented ordinary web upload and the checked Codex CLI loader currently require v1 (1536×1872) and cannot directly use these v2 files. CLI display also depends on terminal graphics support; the IDE extension has no pet picker.

[官方 Pets 说明 / Official Pets guide](https://learn.chatgpt.com/docs/pets) · [桌面安装入口 / Desktop install flow](https://learn.chatgpt.com/docs/reference/commands#pets) · [已核实的 CLI 读取器 / Checked CLI loader](https://github.com/openai/codex/blob/398500106707f0a3217c7cf83edc2bf226cc342f/codex-rs/tui/src/pets/model.rs#L314)
