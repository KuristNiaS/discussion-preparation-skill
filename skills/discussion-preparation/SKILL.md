---
name: discussion-preparation
description: Prepare an academic discussion from a user-confirmed assignment record through strict intake, source verification, complete non-condensing Markdown translation, and synthesis. Use when collecting or verifying assigned materials, translating every part of assigned readings without summary or omission, checking editions and page ranges, explaining academic English for Chinese international students, summarizing texts, extracting people or terms, comparing arguments, or assembling discussion notes from PDFs, DOCX files, screenshots, links, or pasted text.
---

# Discussion Preparation

Build source-grounded discussion notes in three gated phases: obtain the assignment record from the user, deliver complete Markdown translations, then synthesize.

## Audience defaults

When the user is a Chinese international student and gives no conflicting preference:

- Write explanations in clear Chinese suitable for a learner with intermediate academic English.
- Translate assigned readings completely into natural Chinese while retaining important English names, quotations, and technical terms where they support study or citation. Apply the mandatory first-mention rule for titled works in Phase 2.
- Give key concepts as `English term（中文解释）` on first use.
- Make analytical notes Chinese-first and preserve the English wording needed to locate evidence in the source.
- Explain difficult academic phrasing without simplifying the source's argument, evidence, uncertainty, or qualifications.
- Produce discussion analysis rather than a memorized speaking script unless the user explicitly requests one.

## Mandatory opening: ask the user first

At the start of every new discussion-preparation task, ask the user to provide:

- The course topic, week, or discussion theme.
- The complete list of assigned materials, including author, title, edition or publication context, chapter, and printed page range when applicable.
- The source files, paths, links, screenshots, or pasted text available for each item.
- The preferred translation language and any requested outputs beyond translation.

Wait for the user's reply before inspecting local files, browsing, searching, translating, or drafting discussion notes. If the invoking message already contains a material list, ask the user to confirm that the list is complete and authoritative, then wait for confirmation.

Treat the user's confirmed list as the sole assignment record. Local folders, downloads, syllabi, slides, browser state, filenames, and inferred calendar weeks may help locate or verify an item already on that list; they do not define the assignment or add materials to it.

## Phase 1: Complete the source set

### 1. Build and maintain a material inventory

After the user confirms the assignment record, track every listed item with:

- Citation or identifying title.
- Required edition, chapter, and printed page range.
- Source path or URL.
- File readability and actual coverage.
- Translation Markdown path when applicable.
- Status: missing, partial, complete, translated, or summarized.

Keep the inventory internal unless the user asks to see it. Update it whenever the user changes the confirmed list. A newly added assigned item reopens the source and translation gates.

### 2. Resolve missing material

When a listed source or required page is missing:

1. Identify the exact missing item or pages.
2. Search for legitimate free versions only after the user's list establishes that the item is assigned.
3. Prefer public, publisher, library, archival, institutional, public-domain, or openly licensed sources.
4. Use a found source for full translation only when its access and reuse permit that use. Never bypass paywalls, authentication, access controls, or DRM.
5. If no complete, lawfully usable version is available, ask the user to upload the exact missing material and pause at the source gate.

Do not begin summaries, comparisons, discussion questions, or other synthesis while the source gate is open. Do not substitute memory, a different edition, or an unlisted work.

### 3. Verify every source

For each source:

- Confirm author, title, edition or publication context, and chapter.
- Distinguish PDF file pages from printed pages.
- Verify every required printed page is present.
- Check first and last sentences across page boundaries for missing continuations.
- Identify OCR defects, unreadable scans, duplicated pages, and omitted pages.
- Visually inspect rotated, multi-page, or multi-column scans instead of trusting extracted text order. Identify where an assigned item starts and ends when the same file includes adjacent unassigned material.
- Record overlaps between split files and preserve each assigned file's verified coverage without double-counting the overlap in synthesis.
- Record edition or pagination differences explicitly.

Open the translation phase only when every listed reading is present, readable, and covers the required range. If this gate fails, report the exact gap and wait for the missing upload.

## Phase 2: Deliver complete Markdown translations

### 4. Translate the complete assigned set

Read each complete required range and create one `.md` translation file per assigned reading. Use a stable output directory such as `translations/` inside the active workspace, with clear filenames based on author and title.

Translate the text fully rather than sentence-numbering it. Preserve the source's natural paragraph structure and normal continuous reading flow. Here, “sentence-by-sentence translation” means that every source sentence and detail must be represented faithfully; it does not mean placing each sentence in a separate numbered block. Rejoin sentences broken by page boundaries while marking the page transition at the exact location.

Each translation file must:

- Translate the full assigned range without summarizing or omitting content.
- Represent every source sentence and detail faithfully. Natural target-language restructuring is allowed, but condensation, selective paraphrase, and replacement with a summary are not.
- Preserve title, headings, paragraph order, quotations, lists, figure captions, tables when practical, and material footnote markers.
- On the first occurrence of every titled work, reproduce the source's original-language title exactly and leave it untranslated. This applies to films, television works, songs, albums, books, articles, plays, poems, artworks, and comparable named works. A source-metadata line or heading counts as the first occurrence only when it contains the exact original title. After that first occurrence, retain the original title by default; use a concise Chinese reference only when it improves reading flow and still leaves the work unambiguous.
- Translate meaningful figure, map, diagram, and table text; use a structured list or table when reproducing spatial layout is impractical.
- Mark source page boundaries, preferably as `<!-- Source page 87 -->` or a visible page heading when page-level review matters.
- Keep people, organizations, and specialized concepts in the original language alongside the translation when useful; handle titled works with the mandatory first-mention rule above.
- Repair obvious OCR line breaks and hyphenation without changing meaning.
- Mark uncertain readings or translations instead of guessing.
- Continue from the exact unfinished sentence when supplementing an earlier translation.
- Contain only the continuous translation, concise source metadata, and translator notes needed to expose uncertainty; include source text only for requested bilingual output.

Use Markdown by default because it minimizes formatting overhead and is easy to search and convert. Create DOCX, PDF, or XLSX copies only when requested.

### 5. Apply the translation gate

Before producing any summary or discussion synthesis, require all of the following:

- Every assigned reading has its own `.md` translation file.
- Every required page and page transition is represented.
- Translation coverage matches the verified source ranges.
- No source content has been intentionally condensed or dropped.
- Paragraphs read naturally rather than as mechanically separated sentence blocks.
- Unreadable text and unresolved uncertainty are visibly marked.
- Every translation file has been saved and linked to the user.

If the gate fails, continue translation work or pause for the exact missing upload. Do not move to Phase 3. Deliver all completed translation files before starting the next phase.

## Phase 3: Prepare the discussion

Begin this phase only after the translation gate passes. Base outputs on the completed translations and cross-check important claims against the verified sources. Generate only requested components. Default to analytical notes, evidence, terminology, comparisons, and direct answers to assigned questions. Add presentation scripts, ready-to-say classroom remarks, or canned participation language only when the user explicitly requests them.

Generate the components the user requests. Common components include:

### Per-reading summary

- Full English title and author.
- One-sentence central argument.
- Main evidence and reasoning.
- Historical or cultural significance.
- Author's perspective, assumptions, or limitations.

### Names and terminology

- Give personal names in English and Chinese when a conventional Chinese form exists.
- Give uncommon nouns as `English term — 中文解释`.
- Distinguish people, organizations, events, concepts, places, and cultural works.

### Cultural works

- List only films, songs, albums, or books that appear in the verified reading.
- Separate explicit titles from inferred identifications.
- Preserve original-language titles and provide a Chinese translation when useful.

### Cross-reading synthesis

- Compare agreements, tensions, methods, and historical scales.
- Connect evidence across texts without erasing differences between primary and secondary sources.
- When a discussion prompt names a comparator outside the confirmed assignment record, distinguish a course-framework comparison from a textual comparison. State the limitation, avoid line-level claims about the missing text, and request the comparator only when textual comparison is necessary to answer the prompt.
- End with analytical themes or further questions when requested.

## Completion standard

Finish only when the user's confirmed material list is fully represented, the source and translation gates have passed, and every requested discussion deliverable has been produced. Report concise source limitations, missing pages, edition mismatches, and inferred identifications; never present them as verified facts.
