<!-- ═══════════════════════ HEADER ═══════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,14,18,24&height=230&section=header&text=PromptReel&fontSize=72&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Turn%20a%20title%20and%20a%20topic%20into%20a%20vertical%20AI%20story%20video&descSize=18&descAlignY=60" width="100%" alt="PromptReel header" />

<a href="https://github.com/Syed-Muhammad-Tayyab/PromptReel-AI">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=A855F7&center=true&vCenter=true&width=720&lines=Prompt+%E2%86%92+Story+%E2%86%92+Images+%E2%86%92+Voice+%E2%86%92+Video;Script+%2B+Images+%2B+Voiceover+in+one+command;Made+for+TikTok%2C+Reels+%26+YouTube+Shorts;Built+by+Syed+Muhammad+Tayyab" alt="Typing animation" />
</a>

<br/>

<img src="./assets/banner.png" alt="PromptReel banner" width="90%" />

<br/><br/>

<a href="https://github.com/Syed-Muhammad-Tayyab/PromptReel-AI/stargazers"><img src="https://img.shields.io/github/stars/Syed-Muhammad-Tayyab/PromptReel-AI?style=for-the-badge&logo=github&color=a855f7&labelColor=0d1117" alt="Stars" /></a>
<a href="https://github.com/Syed-Muhammad-Tayyab/PromptReel-AI/network/members"><img src="https://img.shields.io/github/forks/Syed-Muhammad-Tayyab/PromptReel-AI?style=for-the-badge&logo=git&color=ec4899&labelColor=0d1117" alt="Forks" /></a>
<a href="https://github.com/Syed-Muhammad-Tayyab/PromptReel-AI/issues"><img src="https://img.shields.io/github/issues/Syed-Muhammad-Tayyab/PromptReel-AI?style=for-the-badge&color=f97316&labelColor=0d1117" alt="Issues" /></a>
<img src="https://img.shields.io/github/last-commit/Syed-Muhammad-Tayyab/PromptReel-AI?style=for-the-badge&color=22c55e&labelColor=0d1117" alt="Last commit" />
<img src="https://img.shields.io/github/repo-size/Syed-Muhammad-Tayyab/PromptReel-AI?style=for-the-badge&color=38bdf8&labelColor=0d1117" alt="Repo size" />

<br/>

<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=white&labelColor=0d1117" alt="React" />
<img src="https://img.shields.io/badge/TypeScript-5.9-3178C6?style=flat-square&logo=typescript&logoColor=white&labelColor=0d1117" alt="TypeScript" />
<img src="https://img.shields.io/badge/Remotion-4.x-0B84F3?style=flat-square&logo=remotion&logoColor=white&labelColor=0d1117" alt="Remotion" />
<img src="https://img.shields.io/badge/OpenAI-Story%20%2B%20Images-412991?style=flat-square&logo=openai&logoColor=white&labelColor=0d1117" alt="OpenAI" />
<img src="https://img.shields.io/badge/ElevenLabs-Voiceover-000000?style=flat-square&logo=elevenlabs&logoColor=white&labelColor=0d1117" alt="ElevenLabs" />
<img src="https://img.shields.io/badge/Bun-CLI-fbf0df?style=flat-square&logo=bun&logoColor=black&labelColor=0d1117" alt="Bun" />
<img src="https://img.shields.io/badge/Format-1080×1920%20@%2030fps-e11d48?style=flat-square&labelColor=0d1117" alt="Format" />

<br/><br/>

<a href="#-quick-start"><b>⚡ Quick Start</b></a> &nbsp;•&nbsp;
<a href="#-how-it-works"><b>🧠 How It Works</b></a> &nbsp;•&nbsp;
<a href="#-project-structure"><b>📂 Structure</b></a> &nbsp;•&nbsp;
<a href="#-generate-your-own-story"><b>🎬 Generate</b></a> &nbsp;•&nbsp;
<a href="#-customization"><b>🎨 Customize</b></a> &nbsp;•&nbsp;
<a href="#-about-the-author"><b>👤 Author</b></a>

</div>

<br/>

---

## ✨ Overview

**PromptReel** is an AI video generator for short-form vertical content. Give it a **story title** and a **topic** (history, ELI5, fun facts, science) and it produces everything a finished reel needs:

| Stage | What happens | Powered by |
| :-- | :-- | :-- |
| 📝 **Script** | Writes a short, hook-first narration for your topic | OpenAI (`gpt-4.1`) |
| 🖼️ **Visuals** | Describes and generates one 1024×1792 image per scene | OpenAI Images |
| 🎙️ **Voiceover** | Narrates each scene with character-level timestamps | ElevenLabs |
| 🧩 **Timeline** | Merges everything into a single `timeline.json` | Custom CLI |
| 🎞️ **Render** | Animated backgrounds, transitions and word-synced subtitles | React + Remotion |

The result is a **1080 × 1920, 30 fps** video, ready for TikTok, Instagram Reels or YouTube Shorts.

---

## 🚀 Features

<table>
  <tr>
    <td width="50%">

🤖 **One-command generation** &nbsp;— title + topic in, full timeline out  
🎙️ **Word-level synced subtitles** &nbsp;— driven by ElevenLabs timestamps  
🌫️ **Scene transitions** &nbsp;— `fade`, `blur` or `none` per slide  
🔍 **Ken-Burns style motion** &nbsp;— scale animations on every background  

   </td>
   <td width="50%">

🧱 **Typed end to end** &nbsp;— Zod schemas for timeline, story and audio  
👀 **Live studio preview** &nbsp;— hot-reload in Remotion Studio  
🗂️ **Multi-story ready** &nbsp;— every folder in `public/content/` becomes a composition  
🎨 **Easy to restyle** &nbsp;— fonts, colors and layout live in plain React components  

   </td>
  </tr>
</table>

---

## 🧠 How It Works

```mermaid
flowchart LR
    A([🧑 Title + Topic]) --> B[📝 Story script<br/>OpenAI]
    B --> C[🧩 Split into scenes<br/>+ image descriptions]
    C --> D[🖼️ Scene images<br/>OpenAI Images]
    C --> E[🎙️ Voiceover + timestamps<br/>ElevenLabs]
    D --> F[(timeline.json)]
    E --> F
    F --> G[🎞️ React + Remotion<br/>composition]
    G --> H([📱 1080×1920 MP4])

    style A fill:#7c3aed,stroke:#a855f7,color:#fff
    style H fill:#ec4899,stroke:#f472b6,color:#fff
    style F fill:#0ea5e9,stroke:#38bdf8,color:#fff
```

The timeline is built from **three blocks**:

| Block | Purpose |
| :-- | :-- |
| `elements` | Slide backgrounds, enter/exit transitions (e.g. blur) and in-slide animations (e.g. scale) |
| `text` | Subtitle text with start/end times and position (`top`, `center`, `bottom`) |
| `audio` | Voiceover clips, time-aligned with the text |

---

## 🛠️ Tech Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=react,ts,nodejs,bun,npm,git,github,vscode&perline=8" alt="Tech stack icons" />

</div>

| Layer | Tools |
| :-- | :-- |
| **Frontend / Video** | React 19, TypeScript, Remotion 4, `@remotion/google-fonts`, `@remotion/animation-utils`, `@remotion/layout-utils` |
| **Validation** | Zod |
| **AI services** | OpenAI (script + images), ElevenLabs (voice + timestamps) |
| **CLI** | Bun, yargs, prompts, ora, chalk, dotenv |
| **Tooling** | ESLint, Prettier, TypeScript strict mode |

---

## 📂 Project Structure

```text
PromptReel-AI/
├── 📁 assets/
│   └── banner.png                  # README banner
├── 📁 cli/
│   ├── cli.ts                      # Interactive generator (npm run gen)
│   ├── service.ts                  # OpenAI + ElevenLabs API calls
│   └── timeline.ts                 # Story → timeline.json builder
├── 📁 public/
│   └── 📁 content/
│       └── 📁 history-of-venus/    # Demo story (one folder per story)
│           ├── descriptor.json     # Script, image prompts, audio timestamps
│           ├── timeline.json       # Final timeline used by the renderer
│           ├── 📁 images/          # Generated scene images (.png)
│           └── 📁 audio/           # Generated voiceover clips (.mp3)
├── 📁 src/
│   ├── 📁 components/
│   │   ├── AIVideo.tsx             # Main composition (intro + scenes + audio)
│   │   ├── Background.tsx          # Image backgrounds, transitions, animation
│   │   ├── Subtitle.tsx            # Subtitle track
│   │   └── Word.tsx                # Animated single word
│   ├── 📁 lib/
│   │   ├── constants.ts            # FPS, intro length, image size
│   │   ├── types.ts                # Zod schemas and TypeScript types
│   │   └── utils.ts                # Timeline loading and frame math
│   ├── Root.tsx                    # Registers one composition per story
│   └── index.ts                    # Entry point
├── .env.example                    # API key template
├── .gitignore
├── .prettierrc
├── eslint.config.mjs
├── package.json
├── remotion.config.ts
├── tsconfig.json
└── README.md
```

---

## ⚡ Quick Start

### Prerequisites

- **Node.js** 18 or newer
- **Bun** (used by the `gen` script) → [bun.sh](https://bun.sh)
- An **OpenAI API key** and an **ElevenLabs API key** *(only needed to generate new stories)*

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Syed-Muhammad-Tayyab/PromptReel-AI.git
cd PromptReel-AI
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Preview the demo story

```bash
npm run dev
```

Remotion Studio opens in your browser with the **History of Venus** demo story.

### 4️⃣ Render to MP4

```bash
npx remotion render history-of-venus out/history-of-venus.mp4
```

> The composition id is the folder name inside `public/content/`.

---

## 🎬 Generate Your Own Story

### 🔑 Configure keys

Create a `.env` file in the project root (a template is in `.env.example`):

```env
OPENAI_API_KEY=your_openai_key
ELEVENLABS_API_KEY=your_elevenlabs_key
```

> If no `.env` is found, the CLI will prompt you for both keys.

### 🗣️ Choose a voice

Open [`cli/service.ts`](cli/service.ts) and change `voiceId` inside `generateVoice()` to any voice from your ElevenLabs library. You can copy the id from the voice URL (the part after `voiceId=`).

### ▶️ Run the generator

```bash
npm run gen
```

You will be asked for:

| Prompt | Example |
| :-- | :-- |
| **Title** | `Why do cats purr?` — can be short or long and detailed |
| **Topic** | `Fun facts`, `History`, `ELI5`, `Science` |

Or skip the prompts with flags:

```bash
npm run gen -- --title "Secrets of the Pyramids" --topic "History"
```

The CLI then creates `public/content/<your-title>/` with the script, images, audio and `timeline.json`. Run `npm run dev` and your new story appears as a composition.

---

## 🎨 Customization

| I want to change… | Edit this |
| :-- | :-- |
| Title card look (font, colors, border) | [`src/components/AIVideo.tsx`](src/components/AIVideo.tsx) |
| Background transitions & motion | [`src/components/Background.tsx`](src/components/Background.tsx) |
| Subtitle style & word animation | [`src/components/Subtitle.tsx`](src/components/Subtitle.tsx), [`src/components/Word.tsx`](src/components/Word.tsx) |
| Video size, FPS, intro length | [`src/lib/constants.ts`](src/lib/constants.ts) |
| How scenes become a timeline | `createTimeLineFromStoryWithDetails()` in [`cli/timeline.ts`](cli/timeline.ts) |
| Story tone & image style prompts | Prompt builders in [`cli/service.ts`](cli/service.ts) |
| Narrator voice | `voiceId` in [`cli/service.ts`](cli/service.ts) |

---

## 🌐 Deploying as a Remote Service

PromptReel renders locally out of the box. To run it as a hosted service:

1. Deploy the Remotion renderer with this project's bundle (`npm run build`).
2. Update [`src/Root.tsx`](src/Root.tsx) to take a **timeline URL as a prop** instead of a local project name.
3. Upload generated images and audio to storage and use their **URLs** in the timeline instead of file names.

---

## 🗺️ Roadmap

- [ ] Web dashboard to enter a title/topic and download the video
- [ ] Multiple voice and visual style presets
- [ ] Urdu / multilingual narration
- [ ] Background music track with auto-ducking
- [ ] One-click upload to YouTube Shorts

---

## 🧯 Troubleshooting

| Problem | Fix |
| :-- | :-- |
| `bun: command not found` | Install Bun from [bun.sh](https://bun.sh), then re-run `npm run gen` |
| `OpenAI error` / `ElevenLabs error` | Check your API keys, billing and rate limits |
| New story not visible in Studio | Make sure `public/content/<story>/timeline.json` exists, then restart `npm run dev` |
| Outdated render packages | Run `npx remotion upgrade` |

---

## 📜 License & Credits

PromptReel is built on top of **[Remotion](https://www.remotion.dev)**. Remotion is free for individuals and small teams, while some companies need a company license, so please check the [Remotion license terms](https://github.com/remotion-dev/remotion/blob/main/LICENSE.md) before using this commercially.

AI services used: **OpenAI** and **ElevenLabs**, each subject to its own terms.

---

## 👤 About the Author

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=800&color=22D3EE&center=true&vCenter=true&width=640&lines=Syed+Muhammad+Tayyab;Full-Stack+Developer+%7C+MERN+Stack;Security-Minded+Engineer;BSCS+%E2%80%A2+Information+Security+%E2%80%A2+FUUAST+Islamabad" alt="Author typing animation" />

<br/><br/>

**Syed Muhammad Tayyab** &nbsp;·&nbsp; 📍 Islamabad, Pakistan  
🎓 BSCS (Information Security) at **FUUAST Islamabad**  
💻 Full-Stack Developer &nbsp;|&nbsp; Security-Minded Engineer &nbsp;|&nbsp; MERN Stack  
🛡️ Cybersecurity interest: SIEM, penetration testing, Red Team

<br/>

<a href="https://github.com/Syed-Muhammad-Tayyab"><img src="https://img.shields.io/badge/GitHub-Syed--Muhammad--Tayyab-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>

<br/><br/>

<img src="https://skillicons.dev/icons?i=html,css,js,react,nodejs,express,php,mysql,mongodb,threejs,git,figma,kali,python&perline=14" alt="Skills" />

<br/><br/>

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Syed-Muhammad-Tayyab&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="GitHub stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Syed-Muhammad-Tayyab&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117" alt="Top languages" />

<br/>

<img src="https://streak-stats.demolab.com?user=Syed-Muhammad-Tayyab&theme=tokyonight&hide_border=true&background=0d1117" alt="GitHub streak" />

</div>

---

## 🤝 Contributing

Ideas and improvements are welcome.

1. Fork the repository
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push the branch: `git push origin feature/my-feature`
5. Open a Pull Request

---

<div align="center">

### ⭐ If PromptReel helped you, give it a star!

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,14,18,24&height=120&section=footer" width="100%" alt="footer" />

<sub>Made with ❤️ by <a href="https://github.com/Syed-Muhammad-Tayyab"><b>Syed Muhammad Tayyab</b></a></sub>

</div>
