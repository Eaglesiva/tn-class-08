# Class 8 Tamil — Book Edition Verification & Scope Audit

- Audit date: 2026-11-06
- Class / Subject / Medium: Class 8 / Tamil / Tamil Medium
- Repository: https://github.com/Eaglesiva/tn-class-08
- Page manifest: `tamil/pages.json` maps the consolidated textbook page set across nine unit folders.
- Question source under active work: `tamil/01_tamil_inbam/book_back_questions/questions.md`

## Correction to the previous audit — false alarm resolved

The earlier audit incorrectly compared the **unit title** with the **title of a poem within that unit**:

- Unit 1 title: **தமிழ் இன்பம்**
- First poem / subsection: **தமிழ்மொழி வாழ்த்து**
- Other contents in the unit, as confirmed by the repository owner: **தமிழ்மொழி மரபு**, **தமிழ் வரிவடிவ வளர்ச்சி**, and **எழுத்துகளின் பிறப்பு**.

These are hierarchical contents of the same unit, not evidence of two different textbook editions. The previous conclusion that the repository might contain an older edition merely because `questions.md` is titled `தமிழ்மொழி வாழ்த்து` was a false alarm and is withdrawn.

## Edition decision

**USER_CONFIRMED_CURRENT_EDITION — ACCEPTED FOR THIS WORKFLOW**

The repository owner explicitly confirmed on 2026-11-06 that the repository's questions are from the currently used Samacheer textbook and clarified the unit / poem title hierarchy. Work must continue using the existing repository source files; do not stop or ask for another PDF solely because the folder / lesson labels differ.

The official Tamil Nadu Textbook and Educational Services Corporation website separately confirms that Class 8 annual textbooks for academic year 2026–27 went on sale from 14-05-2026:
https://www.textbookcorp.in/schools

**Scope note:** This acceptance records the repository owner's edition confirmation for the requested workflow. It does not claim an independently completed official-PDF SHA-256 match or a visual audit of every textbook page. Those are separate evidence checks and must not be confused with the resolved unit-title / poem-title issue.

## Separate content-integrity issue found in Unit 1

During Step 1 source reconciliation, the fourth MCQ in `tamil/01_tamil_inbam/book_back_questions/questions.md` has a likely transcription / extraction defect:

- Repository stem currently reads: `அறிந்து + அனைத்தும்`.
- Repository options B and C are duplicated as `அறிந்தனைத்தும்`.
- Multiple independent secondary answer pages render the textbook question as `அறிந்தது + அனைத்தும்`, with four distinct options, and identify `அறிந்ததனைத்தும்` as the answer:
  - https://www.brainkart.in/article/Poem--Tamil-mozhi-valthu--Questions-and-Answers_11403/
  - https://braingrain.in/grade8-tamil/chapter_01-unit.html
  - https://www.kalviimayam.com/2025/06/8th-tamil-unit-1-book-back-answer.html

This is a **question-data integrity review**, not an edition mismatch. Preserve the original `questions.md` wording until the textbook page is visually checked. In `answers.md`, mark this item `REVIEW_REQUIRED` and do not silently choose an option or rewrite the original file.

## Execution instruction

- Continue with the existing `questions.md` files.
- Follow `docs/BOOK_BACK_QUIZ_WORKFLOW_TA.md`: Step 1 first, then Step 2, then Step 3.
- Do not request the user to upload another textbook PDF as a precondition.
- Record actual unresolved source / transcription conflicts at item level.
- Do not mark a unit COMPLETE while an item needed for Step 1 remains unresolved.
