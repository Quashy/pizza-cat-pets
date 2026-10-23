<p align="center">
  <img src="previews/pizza-pixel.png" alt="披萨 Pizza — a golden cat in a cherry dress, in pixel art" width="256">
</p>

<h1 align="center">披萨 · Pizza</h1>

<p align="center">穿樱桃裙的金渐层小猫，陪你一起工作。<br>A golden cat in a cherry dress, keeping you company while you work.</p>

<p align="center">
  <a href="#create">用自己的宠物制作 · Make your own</a> ·
  <a href="#install">直接使用披萨 · Get Pizza</a> ·
  <a href="#preview">查看两版 · Preview</a>
</p>

<a id="create"></a>
## 有自己的宠物？/ Have a pet of your own?

**你的照片 → 写实与像素形象 → 会动的桌面陪伴**<br>
**Your photos → realistic and pixel characters → an animated desktop companion**

复制 [创建提示词](prompts/create-your-pet.md)，附上少量你有权使用的照片，让 AI 制作 **写实版＋16-bit、128×128 逻辑画布像素版**。先确认主形象，再看动作预览，最后按应用实际能力安装和切换。

Copy the [creation prompt](prompts/create-your-pet.md) and attach a few photos you have permission to use. Your AI will create **a realistic version and a 16-bit pixel version on a 128×128 logical canvas**. Approve the main looks, review the animation, then install and switch using your app's available capabilities.

<a id="install"></a>
## 想直接使用披萨？/ Want Pizza instead?

复制 [安装提示词](prompts/install.md) 给你的 AI。它会检查应用能力，分别安装 **Pizza Original** 和 **Pizza Pixel**，并默认启用写实原版，保留已有宠物。

Copy the [installation prompt](prompts/install.md) to your AI. It will check your app's capabilities, install **Pizza Original** and **Pizza Pixel** separately, and activate the realistic Original by default while preserving existing pets.

之后说 **“切换到像素版披萨”** 或 **“切换到原版披萨”**。两份提示词都内含仓库链接，可独立复制分享。

Then say **“Switch to Pizza Pixel”** or **“Switch to Pizza Original.”** Both prompts include the repository URL and work as standalone requests.

<a id="preview"></a>
## 两种模样，同一个披萨 / Two looks, one Pizza

| 原版 / Original | 像素版 / Pixel |
| :---: | :---: |
| <img src="previews/pizza-original.png" alt="写实版披萨 / Realistic Pizza" width="192"> | <img src="previews/pizza-pixel.png" alt="16-bit像素版披萨 / 16-bit Pixel Pizza" width="192"> |
| 写实毛绒质感，樱桃裙 / Realistic fur, cherry dress | 16-bit 风格，128×128 逻辑画布 / 16-bit style, 128×128 logical canvas |
| <img src="previews/pizza-original.gif" alt="原版披萨动作预览 / Original Pizza animation" width="192"> | <img src="previews/pizza-pixel.gif" alt="像素版披萨动作预览 / Pixel Pizza animation" width="192"> |
| [宠物 PNG / Sprite sheet](pets/original/spritesheet.png) | [宠物 PNG / Sprite sheet](pets/pixel/spritesheet.png) · [原生主图 / Native portrait](previews/pizza-pixel-native.png) |

## 兼容性 / Compatibility

- 两版均为透明 Pets v2 PNG：1536×2288，8列×11行，192×208 单元，9种状态与16个注视方向。128×128 指像素创作画布，不是安装文件尺寸。<br>Both are transparent Pets v2 PNGs: 1536×2288, 8 columns × 11 rows, 192×208 cells, 9 states and 16 look directions. 128×128 describes the pixel artwork, not the install file.
- 需要支持 v2 的桌面宠物安装入口或 Pets 工具。普通 ChatGPT 对话不保证能安装或访问电脑；本地目录安装须核实实际版本与格式。<br>Requires a v2-capable desktop pet install flow or Pets tools. An ordinary ChatGPT chat may not install pets or access your computer. Local folder installation requires verification of the actual version and format.
- 网页普通上传说明及核实到的 Codex CLI 读取器目前仍限定 v1（1536×1872），不能直接使用这里的 v2 文件。CLI 显示还取决于终端图形支持；IDE 扩展没有宠物选择器。<br>The documented ordinary web upload and the checked Codex CLI loader currently require v1 (1536×1872) and cannot directly use these v2 files. CLI display also depends on terminal graphics support; the IDE extension has no pet picker.

[官方 Pets 说明 / Official Pets guide](https://learn.chatgpt.com/docs/pets) · [桌面安装入口 / Desktop install flow](https://learn.chatgpt.com/docs/reference/commands#pets) · [已核实的 CLI 读取器 / Checked CLI loader](https://github.com/openai/codex/blob/398500106707f0a3217c7cf83edc2bf226cc342f/codex-rs/tui/src/pets/model.rs#L314)
