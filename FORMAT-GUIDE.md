# Format Guide — Adding New Answers

Follow this exact structure whenever a new chapter or lesson is added, now or in future sessions.

## File naming
- Lesson: `answers/chapter-{CC}-lesson-{LL}.md` — 2-digit, zero-padded chapter and lesson numbers (e.g. `chapter-02-lesson-03.md`).
- Chapter review/vocabulary: `answers/chapter-{CC}-review-vocabulary.md`
- Chapter test: `answers/chapter-{CC}-test.md`

## Lesson file template
```markdown
# Chapter {C}, Lesson {L}

## Guided Notes
1. <sentence with **bolded fill-in-the-blank answer**>

## Analyze and Reflect   <!-- omit this whole section if the lesson has none -->

**Q1. <question text>**

A: <answer text — copied exactly as given>
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
