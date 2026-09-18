# Localisation QA (working title) - trial builds

Compares the InDesign IDML you sent out for translation with the IDML that came back,
and reports what was lost, what changed structurally, and what looks untranslated -
without opening InDesign. Runs locally; nothing leaves your machine.

**This repository hosts the trial builds only.** The source is not published.

## Download

Latest build: see [Releases](../../releases/latest). Windows 64-bit. Not code-signed yet,
so Windows will warn once on first launch (details in `QUICK_START.md` inside the zip).

## What is in the zip

- `LocalisationQA.exe` - desktop window: pick two IDML files, pick the delivery profile, Compare
- `lqa.exe` - the same engine on the command line
- `stamp_labels.jsx` - run on the document *before* you send it out, so objects can be matched after an InDesign re-export
- `sample/` - a small document pair with planted defects; always reported in full
- `QUICK_START.md`, `LICENSE.txt`

## What the trial shows

The whole document pair is analysed and every finding is counted. One finding per rule is
shown with its location and content; the rest are listed by rule only. The bundled sample
shows the complete report.

## Feedback

I am looking for real before/after pairs from translation round trips, to find out whether
the tool catches anything your current check does not - or flags things that are fine.
Either answer is useful: **hi@linguist-coder.com**.

The call for testers, with more detail on what is checked and what is not:
[Seeking Testers: Comparing IDML Files Before and After Translation](https://www.linguist-coder.com/2026/09/seeking-testers-comparing-idml-files.html).

## Background

- [Comparing InDesign Files After Translation: What to Check](https://www.linguist-coder.com/2026/09/comparing-indesign-files-after.html) - what a structural review covers, and how to do it by hand on the IDML
- [Why IDML Formatting Can Produce Translation Tags, and What to Check in InDesign](https://www.linguist-coder.com/2026/09/why-idml-formatting-can-produce.html) - where the tags in a CAT tool come from
- [Scaling Multilingual DTP by Automating Trados-Ready IDML Export from InDesign Books](https://www.linguist-coder.com/2026/01/scaling-multilingual-dtp-by-automating.html) - preparing the IDML before it goes out

By the author of [Overset Fixer Pro](https://aescripts.com/overset-fixer-pro/) and
[LinkSafe](https://aescripts.com/linksafe/) for InDesign.
