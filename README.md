# Command Line for Biologists

*A Practical Guide to the Terminal, Tools, and Reproducible Workflows*

[![Build PDF](https://github.com/andrewbudge/Command-Line-for-Biologists-Guide/actions/workflows/build.yml/badge.svg)](https://github.com/andrewbudge/Command-Line-for-Biologists-Guide/actions/workflows/build.yml)

> ⚠️ **Work in progress.** This guide is being actively written. Chapters will be added, content will change, and typos absolutely exist. Feedback at this stage is especially welcome.

## 📖 Read the latest draft

**[Download the PDF →](https://github.com/andrewbudge/Command-Line-for-Biologists-Guide/releases/latest)**

The PDF is automatically rebuilt every time the book is updated, so the link above always points to the freshest version.

## Who is this for?

Biologists who aren't computer scientists or bioinformaticians.

If you're a biology student who's been told to "just run this pipeline," a researcher trying to QC your own sequencing data without a dedicated bioinformatics team, or anyone in the life sciences who suspects the command line could save them hours of clicking — this guide is for you. It assumes no prior programming experience and tries hard not to assume you already know the jargon.

## What's covered (and planned)

The book is organized into three parts:

1. **The Terminal.** How to navigate the filesystem, read and search files, compose tools with pipes, manage processes, and edit text — without leaving the keyboard.
2. **Tools.** Common bioinformatics file formats (FASTA, FASTQ, SAM/BAM, VCF), the core toolkit (samtools, seqkit, and friends), installing software cleanly with conda, and working on remote computers and HPC clusters.
3. **Reproducible Workflows.** Shell scripting, organizing a project so future-you can find anything, version control with git, environment management, and a gentle introduction to workflow managers.

The detailed chapter list is still in flux — see the [book source](book/) for what's actually written so far.

## Feedback and contributions

Spotted a typo, a confusing explanation, or a topic that would help? [Open an issue](https://github.com/andrewbudge/Command-Line-for-Biologists-Guide/issues/new) — even half-formed thoughts are useful at this stage. If you'd like to suggest specific edits, pull requests are welcome too.

## How it's built

The book is written in LaTeX, drafted in [Overleaf](https://www.overleaf.com), and synced to this repository. Every push triggers a GitHub Actions workflow that compiles the source and attaches a fresh PDF to the [latest release](https://github.com/andrewbudge/Command-Line-for-Biologists-Guide/releases/latest). If you'd like to build the PDF locally, see [`book/README.md`](book/README.md) for instructions.
