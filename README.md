# AI Contextual B-Roll Injector 🎞️

A prototype automated editor that dramatically speeds up video editing workflows. The script parses speech text into semantic tokens, matches specific visual nouns against a local asset inventory or API, and programmatically layers the matching B-roll footage right over the primary video stream.

### Key Capabilities
- NLP-driven keyword extraction using Speech-to-Text data.
- Layered video timeline compositing.
- Precision timestamps rendering.

## 🎞️ Asset Injection Example

### 📥 Dialogue Input Track
- **Audio Transcript:** "If you want to save **money**, stop wasting time and start writing **code**."

### ⚙️ Semantic Keyphrase Extraction
- **Trigger Word 1:** `"money"` at 00:03s -> Querying database for `finance_stock_clips/`
- **Trigger Word 2:** `"code"` at 00:08s -> Querying database for `developer_matrix_clips/`

### 📤 Composite Output Timeline
- `[00:00 - 00:03]` -> Main speaker visible.
- `[00:03 - 00:06]` -> **B-Roll Overlay:** Crisp 4K footage of coins falling (Main audio continues underneath).
- `[00:06 - 00:08]` -> Timeline switches back to the main speaker.
- `[00:08 - 00:11]` -> **B-Roll Overlay:** Neon glowing terminal screen typing script loops.
