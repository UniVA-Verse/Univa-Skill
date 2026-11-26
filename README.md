<div align="center">

<a href="https://univa.online">
  <img src="docs/assets/readme/Univa-skill.png" alt="UniVA Skill — Harnessing skills as the technical core" width="92%" />
</a>

<br /><br />

<p>
  <strong>A skill-governed runtime for agentic video and audio production.</strong><br />
  <sub>Creative direction, MCP tool contracts, human review gates, and a local timeline studio — unified in one repository.</sub>
</p>

<p>
  <a href="https://univa.online"><img src="https://img.shields.io/badge/Website-univa.online-18181b?style=flat-square&labelColor=09090b" alt="Website" /></a>
  <a href="https://arxiv.org/abs/2511.08521"><img src="https://img.shields.io/badge/Paper-arXiv%202511.08521-18181b?style=flat-square&labelColor=09090b" alt="Paper" /></a>
  <a href="https://huggingface.co/datasets/UniVA-Agent/UniVA-Bench"><img src="https://img.shields.io/badge/Benchmark-UniVA--Bench-18181b?style=flat-square&labelColor=09090b" alt="Benchmark" /></a>
  <a href="https://huggingface.co/spaces/UniVA-Agent/UniVA-Leaderboard"><img src="https://img.shields.io/badge/Leaderboard-HuggingFace-18181b?style=flat-square&labelColor=09090b" alt="Leaderboard" /></a>
  <a href="https://discord.gg/85GkGW897V"><img src="https://img.shields.io/badge/Community-Discord-18181b?style=flat-square&labelColor=09090b" alt="Discord" /></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-18181b?style=flat-square&labelColor=09090b" alt="MIT License" /></a>
</p>

<p>
  <strong>English</strong> &nbsp;·&nbsp; <a href="README.zh-CN.md">简体中文</a>
</p>

<p>
  <sub>
    <a href="#selected-films">Selected Films</a> &nbsp;/&nbsp;
    <a href="#skills-as-the-technical-core">Design Thesis</a> &nbsp;/&nbsp;
    <a href="#anatomy-of-a-reviewed-run">Review Gate</a> &nbsp;/&nbsp;
    <a href="#architecture">Architecture</a> &nbsp;/&nbsp;
    <a href="#pipelines">Pipelines</a> &nbsp;/&nbsp;
    <a href="#local-web-studio">Web Studio</a> &nbsp;/&nbsp;
    <a href="#quickstart">Quickstart</a> &nbsp;/&nbsp;
    <a href="#citation">Citation</a>
  </sub>
</p>

</div>

---

## Selected Films

> **Three films. One skill graph.** Real multi-shot pieces planned, reviewed, generated, scored, and assembled end-to-end with UniVA Skill. Click any frame to play, or open the offline screening dossier at [`docs/showcase/index.html`](docs/showcase/index.html).

<table>
  <tr>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/skill-films/ink.mp4">
        <img src="docs/assets/readme/skill-films/ink.jpg" alt="A Crane Opens the Mountains" width="100%" />
      </a>
      <br />
      <sub><code>01</code> &nbsp;·&nbsp; INK / SPATIAL FANTASY &nbsp;·&nbsp; 20s</sub><br />
      <strong>A Crane Opens the Mountains</strong><br />
      <sub>Directed with <code>chinese-ink-guochao</code>, multi-shot storyboard review, and layered wind/water sound design.</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/skill-films/story.mp4">
        <img src="docs/assets/readme/skill-films/story.jpg" alt="The Last Light" width="100%" />
      </a>
      <br />
      <sub><code>02</code> &nbsp;·&nbsp; SCI-FI / NARRATIVE &nbsp;·&nbsp; 20s</sub><br />
      <strong>The Last Light</strong><br />
      <sub>Built through <code>story-video</code>, energy-arc pacing, visual continuity locks, and atmospheric scoring.</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/skill-films/product.mp4">
        <img src="docs/assets/readme/skill-films/product.jpg" alt="IOTA ONE · Precision in Motion" width="100%" />
      </a>
      <br />
      <sub><code>03</code> &nbsp;·&nbsp; INDUSTRIAL / PRODUCT &nbsp;·&nbsp; 20s</sub><br />
      <strong>IOTA ONE · Precision in Motion</strong><br />
      <sub>Crafted via <code>product-advertising</code>, styleframe lighting constraints, and tactile acoustic accents.</sub>
    </td>
  </tr>
</table>

<details>
<summary>Archive reels &amp; editor exports (6 additional works)</summary>
<br />

<table>
  <tr>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/tokyo-olympics-promo-with-audio.mp4">
        <img src="docs/assets/readme/olympics.png" alt="Sports Promo" width="100%" />
      </a>
      <br /><strong>Sports Promo</strong><br /><sub>Multi-shot sequence with BGM &amp; SFX</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/stadium-crowd-story.mp4">
        <img src="docs/assets/readme/smooth-crossfade-poster.jpg" alt="Stadium Crowd" width="100%" />
      </a>
      <br /><strong>Stadium Crowd</strong><br /><sub>Continuity assembly with xfade transitions</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/desert-car.mp4">
        <img src="docs/assets/readme/desert.png" alt="Desert Drive" width="100%" />
      </a>
      <br /><strong>Desert Drive</strong><br /><sub>Wide cinematic automotive study</sub>
    </td>
  </tr>
  <tr>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/ev-ad-captioned.mp4">
        <img src="docs/assets/readme/ev-ad-poster.jpg" alt="EV Commercial" width="100%" />
      </a>
      <br /><strong>EV Commercial</strong><br /><sub>Commercial cut with timed captions</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/anime-fight-captioned.mp4">
        <img src="docs/assets/readme/anime-fight-poster.jpg" alt="Anime Action Short" width="100%" />
      </a>
      <br /><strong>Anime Action Short</strong><br /><sub>Dynamic multi-shot action + caption overlay</sub>
    </td>
    <td width="33.33%" align="left" valign="top">
      <a href="docs/assets/readme/editor-basics-demo.mp4">
        <img src="docs/assets/readme/editor-basics-preview.png" alt="Local Web Studio Export" width="100%" />
      </a>
      <br /><strong>Local Web Studio Export</strong><br /><sub>Browser WebCodecs MP4 render (<a href="docs/assets/readme/editor-basics-workflow.webm">workflow capture</a>)</sub>
    </td>
  </tr>
</table>

<sub>Audio attributions for demo films are documented in [`docs/assets/readme/skill-films/CREDITS.md`](docs/assets/readme/skill-films/CREDITS.md).</sub>
</details>

---

## Skills as the Technical Core

Most AI video tools bind creative logic to prompts hidden inside a single web app. **UniVA Skill** inverts that model: creative craft, tool contracts, review governance, and orchestration live as versioned Markdown and YAML inside the repository itself.

<table>
  <tr>
    <td width="50%" valign="top">
      <strong>One Skill Graph, Every Surface</strong><br />
      <sub>Codex, Claude Code, terminal coding agents, the FastAPI backend, and the local Web Studio all execute against the exact same <code>skills/</code> tree and MCP tool contracts.</sub>
    </td>
    <td width="50%" valign="top">
      <strong>Review Before Render</strong><br />
      <sub>Every generation or editing task pauses at an explicit <code>awaiting_human</code> gate with inspectable JSON plans, prompts, constraints, and budgets before any paid media call executes.</sub>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <strong>Contract-Driven Media Tools</strong><br />
      <sub>34 active MCP tools across 7 servers are specified in <code>skills/core/</code> with strict parameter schemas, defaults, output policies, and failure semantics — decoupled from any single vendor.</sub>
    </td>
    <td width="50%" valign="top">
      <strong>Provenance &amp; Persistent Taste</strong><br />
      <sub>Runs emit approval hashes, cost receipts, and verified <code>delivery_report.json</code> records, while reusable directorial preferences persist locally in <code>skills/user/</code>.</sub>
    </td>
  </tr>
</table>

---

## Anatomy of a Reviewed Run

Rather than firing blind API requests from a one-line prompt, UniVA enforces a **two-phase plan-and-execute lifecycle** governed by [`skills/meta/media-review-gate.md`](skills/meta/media-review-gate.md):

```text
PHASE 01 · PLAN & REVIEW (zero generation spend)
────────────────────────────────────────────────────────────────────────────────
  User Brief            "A three-shot Chinese ink-wash short with wind & water ambience."
     │
     ├─ Skill Loading   master router → story-video + chinese-ink-guochao + creative/*
     ├─ Planning        research_brief.json  →  shot_plan.json (camera, light, pacing, audio)
     ├─ Validation      prompt-validator & creative-quality-gate  →  storyboard_validation.json
     └─ Human Gate      emits storyboard_review.json  →  HALTS at `awaiting_human`

PHASE 02 · APPROVED EXECUTION & DELIVERY (runs only after explicit sign-off)
────────────────────────────────────────────────────────────────────────────────
  Approved Plan         --approved-plan <run_dir>/shot_plan.json
     │
     ├─ Exact Binding   calls MCP tools strictly with approved expanded prompts & parameters
     ├─ Sound Design    native API audio → dedicated audio API (BGM/SFX) → FFmpeg fallback
     ├─ Assembly        FFmpeg xfade merge + optional Remotion title/caption packaging
     └─ Verification    probes real media streams, hashes & receipts  →  delivery_report.json
```

> **Audio Discipline:** Default video delivery includes non-voice audio (BGM, ambience, SFX, transitions). Voiceover, dubbing, or spoken dialogue is generated only when explicitly requested.

---

## Architecture

UniVA organizes **101 skill specifications**, **7 declarative YAML pipelines**, and **34 active MCP tools** into three cleanly separated layers — click the reel below to watch the full **1080p film with sound** ([`architecture-film.mp4`](docs/assets/readme/architecture-film.mp4)).

<p align="center">
  <a href="docs/assets/readme/architecture-film.mp4">
    <img src="docs/assets/readme/architecture-preview.webp" alt="UniVA Skill — Three-Layer Architecture Film (Click for 1080p MP4 with audio)" width="100%" />
  </a>
  <br />
  <sub>
    <strong>Architecture in Motion</strong> &nbsp;·&nbsp; 28s &nbsp;·&nbsp; 1920×1080 &nbsp;·&nbsp;
    <a href="docs/assets/readme/architecture-film.mp4">Watch full 1080p film with audio</a>
  </sub>
</p>

| Layer | Directory | Responsibility |
| :--- | :--- | :--- |
| **Control Surfaces** | `AGENTS.md` · `CLAUDE.md` · `univa/` · `apps/web/` | Codex, Claude Code, terminal agents, FastAPI backend, and Local Web Studio — all reading one skill graph |
| **Layer 03 · Orchestration** | `pipeline_defs/*.yaml` · `skills/pipelines/` | 7 declarative YAML pipelines and 23 stage directors routing intent from brief to final composition |
| **Layer 02 · Craft & Governance** | `skills/creative/` · `skills/themes/` · `skills/meta/` · `skills/user/` | 18 creative skills, 20 auto-triggered theme enhancers, 23 meta protocols (`awaiting_human` gate, provenance), and user preferences |
| **Layer 01 · Atomic Contracts** | `skills/core/` · `univa/mcp_tools/` | 12 core contract specs governing 7 MCP servers and 34 active media tools, finishing via FFmpeg &amp; Remotion |

---

## Pipelines

All workflows are declared transparently in `pipeline_defs/` and orchestrated by stage director skills in `skills/pipelines/`.

| Pipeline | Manifest | Lifecycle | Gate |
| :--- | :--- | :--- | :---: |
| **Master Router** | [`master.yaml`](pipeline_defs/master.yaml) | Classifies user intent, routes to a specialized pipeline, or synthesizes a dynamic plan | `guided` |
| **Story Video** | [`story-video.yaml`](pipeline_defs/story-video.yaml) | Idea → Script → Scene Plan → Character/Keyframe Assets → Multi-Shot Edit → Compose | `guided` |
| **Creative Proposal** | [`creative-proposal.yaml`](pipeline_defs/creative-proposal.yaml) | Generates 2–3 distinct creative directions → user selection → shot-by-shot storyboard → render | `guided` |
| **Video Edit** | [`video-edit.yaml`](pipeline_defs/video-edit.yaml) | Analyze source → propose edits → approve → execute (style, repaint, depth, pose) → iterate | `guided` |
| **Video Understand** | [`video-understand.yaml`](pipeline_defs/video-understand.yaml) | Durable time-coded media index → multi-dimensional analysis → structured report & refinement | `guided` |
| **Localization** | [`localization.yaml`](pipeline_defs/localization.yaml) | ASR transcription → subtitle translation → bilingual captions → optional dubbing → locale QA | `strict` |
| **Media Atomic** | [`media-atomic.yaml`](pipeline_defs/media-atomic.yaml) | Compact reviewed lane for standalone images, sequential images, BGM/SFX, and speech | `strict` |

---

## Technical Reference

<details>
<summary><strong>MCP Tool Matrix</strong> — 7 servers, 34 active tools &amp; contract sources</summary>
<br />

At execution time, function signatures, defaults, output policies, and failure shapes are sourced directly from [`skills/INDEX.md`](skills/INDEX.md) and `skills/core/*.md`:

| MCP Server | Contract Specification | Active Tools |
| :--- | :--- | :--- |
| `video_gen` | [`wavespeed-video-gen.md`](skills/core/wavespeed-video-gen.md) · [`ffmpeg-merge.md`](skills/core/ffmpeg-merge.md) · [`remotion-compose.md`](skills/core/remotion-compose.md) | `plan_video_shots`, `text2video_gen`, `image2video_gen`, `frame2frame_video_gen`, `video_extension`, `storyvideo_gen`, `entity2video`, `merge2videos`, `remotion_compose_video` |
| `image_gen` | [`wavespeed-image-gen.md`](skills/core/wavespeed-image-gen.md) | `text2image_generate`, `image2image_generate`, `sequential_image_gen` |
| `video_editing` | [`video-editing.md`](skills/core/video-editing.md) · [`ark-video-reference-upload.md`](skills/core/ark-video-reference-upload.md) | `depth_modify`, `style_transfer`, `repainting`, `pose_reference` |
| `video_understanding` | [`video-understanding.md`](skills/core/video-understanding.md) · [`media-index.md`](skills/core/media-index.md) | `vision2text_gen`, `index_video_media`, `update_video_index_segments`, `search_video_moments`, `get_video_moment` |
| `video_tracking` | [`video-tracking.md`](skills/core/video-tracking.md) | `video_referring_segmentation` |
| `audio_gen` | [`audio-gen.md`](skills/core/audio-gen.md) | `plan_audio_for_video`, `audio_gen`, `speech_gen`, `generate_audio_assets_from_plan`, `mux_audio_timeline` |
| `localization` | [`localization.md`](skills/core/localization.md) | `transcribe_media`, `translate_captions`, `prepare_localized_captions`, `generate_localized_voiceover`, `render_localized_video`, `validate_localized_media` |

</details>

<details>
<summary><strong>Theme Quality Enhancers</strong> — 20 domain-specific cinematography &amp; audio overlays</summary>
<br />

Loaded automatically from task triggers to elevate framing, lighting, rhythm, and sound design without modifying safety policies, review gates, or tool contracts:

| Narrative &amp; Aesthetic | Commercial &amp; Brand | Knowledge &amp; Lifestyle |
| :--- | :--- | :--- |
| `chinese-ink-guochao` | `product-advertising` | `science-explainer` |
| `scifi-anime` | `tech-product-review` | `children-education` |
| `comic-style` | `corporate-promo` | `adult-education-training` |
| `realistic-human-closeup` | `automotive-mobility` | `food-cooking` |
| `gaming-esports` | `fashion-beauty` | `travel-landscape` |
| `festival-celebration` | `real-estate-home` | `sports-fitness` |
| — | `finance-business` | `medical-health` |

</details>

<details>
<summary><strong>Providers &amp; Local Models</strong> — cloud APIs and self-hosted checkpoints</summary>
<br />

Configure only the capabilities you need in `.env` (template: [`.env.example`](.env.example); non-sensitive defaults: [`univa/config/mcp_tools_config/config.yaml`](univa/config/mcp_tools_config/config.yaml)):

- **Planning &amp; Acting LLMs:** DeepSeek (`deepseek-reasoner`), DashScope Qwen, OpenAI, or local OpenAI-compatible endpoints (vLLM / Ollama).
- **Video &amp; Image Generation:** Volcengine Ark (`doubao-seedance-2-0`), Wavespeed (`seedance-v1-pro`, `flux-kontext-pro`, `seedream-v4`, MiniMax `hailuo-02`).
- **Video Editing:** Volcengine Ark (`doubao-seedance-2-0`), Runway (`gen4-aleph`), Wavespeed (`wan-2.1-14b-vace`), or local Wan2.1 / VACE checkpoints.
- **Audio &amp; Speech:** Wavespeed (`mmaudio-v2`) for BGM/SFX/ambience, MiniMax (`speech-2.5-turbo-preview`) for speech, with FFmpeg fallback.
- **Understanding, Retrieval &amp; Tracking:** Cloud VLM (`qwen-vl-max`) or local checkpoints (`Qwen2.5-VL`, `BGE-VL`, `Sa2VA`, `SAM 2`).
- **Packaging:** FFmpeg xfade/audio muxing and optional Remotion composition (`packages/remotion-compose`).

</details>

<details>
<summary><strong>Repository Structure</strong> — layout of skills, pipelines, runtime, and studio</summary>
<br />

```text
univa-skill/
├── skills/                     # 101 Markdown skills indexed by skills/INDEX.md
│   ├── core/                   # 12 MCP tool contract specifications
│   ├── creative/               # 18 creative direction, storyboard, and sound craft skills
│   ├── themes/                 # 20 genre quality enhancers
│   ├── meta/                   # 23 governance, review gate, provenance, and preference protocols
│   ├── pipelines/              # 23 stage director skills paired with pipeline_defs/*.yaml
│   ├── agent-integrations/     # Guides for Codex, Claude Code, and terminal-first agents
│   └── user/                   # Repo-local persistent user preferences
├── pipeline_defs/              # 7 declarative YAML pipeline manifests
├── univa/                      # Python runtime, FastAPI server, and 7 MCP servers
├── apps/web/                   # Local Web Studio (Next.js 15, IndexedDB, WebCodecs export)
├── packages/                   # Shared workspace packages including Remotion packaging
├── scripts/                    # Direct runners, MCP configurator, preflight, and repo checks
└── docs/                       # Offline Skill Films showcase and platform setup guides
```

</details>

---

## Local Web Studio

Paired with the agent runtime is a **browser-native timeline editor** under `apps/web` that runs completely locally — **no database, Redis, telemetry, or provider API keys required** for editing and export.

- **Editing Craft:** Multi-track timeline, media library, shape and image stickers, 6 filters, color adjustment, blur/vignette, 4 transitions, adjustable freeze frames, manual and SRT/VTT captions, and full undo/redo.
- **Deterministic Export:** Projects persist in browser IndexedDB; preview and MP4 export share identical frame composition via WebCodecs (verified on desktop Chrome).
- **Optional AI Chat Bridge:** Run `univa.univa_server` alongside the studio to plan, review, generate, and import assets directly into your timeline.

---

## Quickstart

Requires **Python 3.10+** and **FFmpeg / ffprobe** ([platform setup reference](docs/local-setup-reference.md#quickstart)). **Bun** is required only if you run the Local Web Studio.

### 1. Agent-First Production (No Backend Required)

```bash
git clone https://github.com/univa-agent/univa-skill.git
cd univa-skill

python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.runtime.txt

cp .env.example .env                    # add keys for the providers you intend to use
python scripts/configure_mcp_servers.py
python scripts/preflight_media_runtime.py
```

Open this repository in **Codex**, **Claude Code**, or another coding agent, ask it to read [`AGENTS.md`](AGENTS.md) (or [`CLAUDE.md`](CLAUDE.md)), and describe what you want to make:

```text
Create a three-shot Chinese ink-wash short film with wind and water ambience.
Analyze this video's story structure, camera language, and editing rhythm.
Convert this clip to watercolor animation while preserving motion and framing.
Save a preference: restrained lighting, smooth camera movement, no voiceover.
```

<sub>Integration playbooks: [Codex Video Ops](skills/agent-integrations/codex-univa-video-ops/SKILL.md) · [Claude Code](skills/agent-integrations/claude-code-univa-video-ops/SKILL.md) · [External Agent Bridge](skills/agent-integrations/univa-external-agent-bridge/SKILL.md) · [Artifact Provenance](skills/meta/artifact-provenance.md)</sub>

### 2. Local Web Studio (Zero API Keys)

```bash
bun install
bun run --cwd apps/web dev:local
```

Open **`http://127.0.0.1:3000/projects`** in desktop Chrome.

### 3. Optional · Connect AI Chat Backend

After completing the Python setup above, start the backend server in a second terminal:

```bash
source .venv/bin/activate
UNIVA_SERVER_HOST=127.0.0.1 AUTH_ENABLED=false python -m univa.univa_server
```

---

## Verification & Hygiene

Run formatting, type checking, local production build, and publication checks (secret scan, git-ignore hygiene, and document link verification) without calling external media providers:

```bash
bun run lint
bun run check-types
bun run build:local
bun run check:repo
```

Local secrets (`.env`), generated MCP configurations, caches, logs, and intermediate renders are git-ignored. Commit `.env.example` templates and regenerate MCP configs per machine via `python scripts/configure_mcp_servers.py`.

---

## Citation

If UniVA or UniVA Skill contributes to your research or production workflow, please cite:

```bibtex
@article{liang2025univa,
  title   = {UniVA: Universal Video Agent towards Open-Source Next-Generation Video Generalist},
  author  = {Liang, Zhengyang and Zhang, Daoan and Zhou, Huichi and Huang, Rui and Li, Bobo and Zhang, Yuechen and Wu, Shengqiong and Wang, Xiaohan and Luo, Jiebo and Liao, Lizi and Fei, Hao},
  journal = {arXiv preprint arXiv:2511.08521},
  year    = {2025}
}
```

---

<div align="center">
  <sub>
    <a href="LICENSE">MIT License</a> &nbsp;·&nbsp;
    <a href="docs/assets/readme/skill-films/CREDITS.md">Demo Credits</a> &nbsp;·&nbsp;
    <a href="https://discord.gg/85GkGW897V">Discord</a> &nbsp;·&nbsp;
    <a href="https://univa.online">univa.online</a>
  </sub>
</div>
