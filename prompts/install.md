# 安装与切换披萨 / Install & switch Pizza

复制以下任一语言的完整代码块即可；仓库链接已包含在内。<br>
Copy one complete block below; the repository URL is already included.

## 中文

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

## English

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

能力依据 / Capability references: [Pets](https://learn.chatgpt.com/docs/pets) · [Desktop install flow](https://learn.chatgpt.com/docs/reference/commands#pets). Availability varies by app, account, workspace, and version.
