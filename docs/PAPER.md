# B.A.D.D.I.E. — Academic Research Paper

This directory contains the complete ACM-format research paper for the B.A.D.D.I.E. project.

## Paper Details

- **Title**: B.A.D.D.I.E.: Behavioural Architectures for Digitally-Defined Independent Entities
- **Format**: ACM sigconf (2-column proceedings)
- **Citation Style**: APA 7th Edition
- **Author**: Amir Hafizi Bin Musa (2024745815)
- **Affiliation**: Universiti Teknologi MARA (UiTM) Perak, Tapah Campus, Malaysia

## Files

| File | Description |
|------|-------------|
| `main.tex` | Full LaTeX source |
| `references.bib` | Bibliography (20 references) |

## Abstract

The rapid advancement of large language models (LLMs) has catalyzed a new class of AI systems capable of simulating human-like companionship, personality, and task-oriented assistance. We present B.A.D.D.I.E., a local-first desktop AI companion system that integrates multimodal perception, retrieval-augmented generation (RAG), real-time voice interaction, and an animated Live2D avatar within a unified behavioural architecture. Unlike cloud-dependent assistants, B.A.D.D.I.E. operates entirely on consumer hardware, prioritizing user privacy while delivering a persistent, personality-consistent companion experience.

## Building the PDF

```bash
# Using pdflatex
pdflatex main.tex
bibtex main
pdflatex main.tex
pdflatex main.tex

# Or using latexmk
latexmk -pdf main.tex
```

## Sections

1. **Introduction** — Motivation and contributions
2. **Related Work** — Personality modelling, RAG/memory, voice pipelines, embodiment
3. **System Architecture** — Design principles, core agent, personality pipeline, memory, voice, vision, avatar
4. **Implementation** — Technology stack, local-first considerations
5. **Discussion** — Behavioural implications, privacy/ethics, limitations
6. **Conclusion** — Summary and future directions
