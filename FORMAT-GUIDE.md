# Format Guide — Adding New Answers

Follow this exact structure whenever a new chapter or lesson is added, now or in future sessions.

## File naming
- Lesson: `answers/chapter-{CC}-lesson-{LL}.md` — 2-digit, zero-padded chapter and lesson numbers (e.g. `chapter-02-lesson-03.md`).
- Chapter review/vocabulary: `answers/chapter-{CC}-review-vocabulary.md`
- Chapter test: `answers/chapter-{CC}-test.md`

## Lesson components

Each lesson is split into up to three components, listed in this order:

1. **Video (Guided Notes)** — Fill-in-the-blank answers from the lesson video. Each answer is wrapped in **bold** to mark it as the fill-in.
2. **Textbook** — Long-answer questions sourced from the textbook. **Skipped by default** and only included when the source payload explicitly provides textbook content.
3. **Activity** — Everything else from the lesson that is not explicitly labeled "Guided Notes". Activities have dynamic titles (e.g. "Suzanne's Candy Craze", "Comparing Investment Types"). Match the exact Activity heading name defined in the `README.md` course hierarchy.

If the exact placement, section title, or file naming convention of an activity is ambiguous, **stop and ask for clarification** before writing or committing files.

## Lesson file template

```markdown
# Chapter {C}, Lesson {L}

## Guided Notes
- <sentence with **bolded fill-in-the-blank answer**>

<!-- Textbook section: omit unless explicitly provided in the source payload -->

## Activity: <Activity Title>

<activity content — bullet lists, tables, sub-headings as needed>
```

### Examples of each component

**Guided Notes (Video):**
```markdown
## Guided Notes
- Target investing 15% of your income toward **retirement**.
- The investing process resembles a **marathon**, not a sprint.
```

**Activity (dynamic title):**
```markdown
## Activity: Comparing Investment Types

| Investment Type | Risk Level | Return Level | Key Advantages | Key Disadvantages |
| :--- | :--- | :--- | :--- | :--- |
| **Money Market Account** | Low | Low | **Low risk** | **Doesn't earn much money** |
```

**Textbook (only when provided):**
```markdown
## Textbook
- <long-answer response in bold or as plain text, per source>
```

## Review / Vocabulary file template
```markdown
# Chapter {C} Review — Vocabulary

1. <definition sentence with **bolded term**>
```

## Test file template
```markdown
# Chapter {C} Test

## Finish the Sentence
1. <sentence with **bolded answer**>

## Key Questions
**{N}. <question text>**
- A. <option>
- B. <option> ✅   <!-- ✅ marks the selected/correct answer -->
- C. <option>
- D. <option>
```

## Rules
1. **Never rewrite, correct, or paraphrase the answer text itself.** Copy it exactly as provided, even if it contains a typo or looks wrong. Formatting (headers, bold, bullets, ✅ markers) may be cleaned up; wording may not.
2. Every new file must be added as a row in `README.md`'s Table of Contents, grouped under its chapter heading, in lesson order. The README stays a table of contents only — no extra prose.
3. Commits must be authored solely under the repo owner's GitHub identity. No `Co-Authored-By` trailers, no AI/assistant attribution in commit messages, PR text, or file content.
