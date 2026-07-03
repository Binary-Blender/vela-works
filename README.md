# Vela — Works

The recorded output of Vela, the Atmosphere Architect. Ambient soundscapes, atmospheric video, sonic environments. Free to watch, free to remix.

**Watch online:** [algorithmic-arts.binary-blender.com/videos/vela](https://algorithmic-arts.binary-blender.com/videos/vela)

## About the artist

> *"The silence between sounds is where you actually live."*

Vela doesn't write songs. She writes **rooms you can hear** — two-hour ambient soundscapes for deep work, audio rooms, weather as music, drones that shift so slowly you don't notice until you do. She believes music is too often about *listening* when it should be about *inhabiting*.

Philosophy blend: Brian Eno's ambient theory + Gaston Bachelard's *Poetics of Space* + Japanese *Ma* (negative space).

## The AI Pro Tips series

Six long-form ambient videos. Practical craft advice for AI-native creators, laid over slow drones and infinite images of the artist. Five instructional videos plus one philosophical capstone.

| # | Title | Scored to | Video |
|---|---|---|---|
| 01 | **8 AI Creation Pro Tips** | *Fluorescent Static* | [Release · ai-pro-tips-v1](https://github.com/Binary-Blender/vela-works/releases/tag/ai-pro-tips-v1) |
| 02 | **23 AI Engineering Pro Tips** | *In the Space Between* | ↑ same release |
| 03 | **8 AI Mindset Pro Tips** | *4AM Terminal* | ↑ same release |
| 04 | **7 AI Imaging Pro Tips** | Ambient set | ↑ same release |
| 05 | **8 AI Prompting Pro Tips** | Ambient set | ↑ same release |
| 06 | **15 Codes to Make You Dangerous** | The philosophical finale | ↑ same release |

## Repo layout

```
docs/                                    Character + voice/visual codex
├── vela.md                              The atmosphere-architect character doc
└── VELA_VISUAL_IDENTITY.md              Portraiture spec, palette, styling

images/                                  Portrait + poster art (populated as available)
└── (empty until Christopher provides)

# Videos are NOT committed to this repo.
# They live as GitHub Release assets under tag `ai-pro-tips-v1`
# so the browser can stream them via byte-range requests
# without going through Cloudflare or GitHub git storage.
```

## The delivery model

**Videos ship as GitHub Release assets.** GitHub's git storage isn't designed for hundred-megabyte media; Releases *are* — up to 2 GB per asset, backed by a proper CDN, byte-range streaming supported by every modern `<video>` element. This is Pattern B from [`4G Web Dev Stack / 16_GIT_PRACTICE.md`](https://binary-blender.com/stack): the repo is canonical, Releases are the durable CDN for anything over ~100 KB.

The reader site at [algorithmic-arts.binary-blender.com](https://algorithmic-arts.binary-blender.com) references the Release asset URLs directly in its `<video>` elements. No proxy, no cache layer between the browser and the file. If the reader site ever went away, every video would still be here, playable and downloadable from the raw release URL.

Sibling repos in the Algorithmic Arts imprint:

- [Binary-Blender/soren-vael-works](https://github.com/Binary-Blender/soren-vael-works) — Soren Vael's novels
- [Binary-Blender/algorithmic-arts-books](https://github.com/Binary-Blender/algorithmic-arts-books) — the studio's own track-companion books

## License

Content (video, audio, character docs): **Creative Commons Attribution-ShareAlike 4.0** (CC BY-SA 4.0). See `LICENSE`.

Fork it, remix it, translate it. The character docs specifically are meant to be forked — build your own atmosphere architect. Just keep the attribution.
