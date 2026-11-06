# Class 8 Tamil — Batch Workflow QA Report

- Date: 2026-11-06
- Repository: https://github.com/Eaglesiva/tn-class-08
- Scope: Tamil, Units 1–9
- Batch 1: Units 1–5
- Batch 2: Units 6–9

## Files created

Each of the nine unit folders now has:
- `book_back_questions/answers.md`
- `book_back_questions/quiz.md`
- `book_back_questions/quiz.json`

Master file:
- `tamil/book_back_questions/quiz.json`

## Unit record counts

| Unit | Title | quiz.md questions | quiz.json records |
|---:|---|---:|---:|
| 1 | தமிழ் இன்பம் | 17 | 17 |
| 2 | ஈடில்லா இயற்கை | 16 | 16 |
| 3 | அறிவியல் தொழில்நுட்பம் | 14 | 14 |
| 4 | கல்வி | 12 | 12 |
| 5 | கலை அழகியல் பண்பாடு | 12 | 12 |
| 6 | நாகரிகம் தொழில் வணிகம் | 14 | 14 |
| 7 | நாடு சமூகம் | 10 | 10 |
| 8 | அறம் தத்துவம் சிந்தனை | 14 | 14 |
| 9 | மனிதம் ஆளுமை | 14 | 14 |
| **Total** | | **123** | **123** |

## JSON and synchronization checks

- All nine unit `quiz.json` files parsed successfully.
- Total unit records inspected: 123.
- IDs were unique across all 123 unit records.
- Every record inspected had exactly four options.
- Correct-answer indices were integer values from 0 through 3.
- Required ID / question / source fields were present.
- Every unit's `quiz.md` numbered-question count matched its `quiz.json` record count.
- Two records had duplicate option text and were flagged `REVIEW_REQUIRED_DUPLICATE_OPTIONS`:
  - Unit 2: `8_tam_u2_q4`
  - Unit 9: `8_tam_u9_q8`
- One additional Unit 9 record, `8_tam_u9_q13`, remains `REVIEW_REQUIRED` because the answer wording needs source confirmation.
- The three review-required records were excluded from the Master Quiz.
- Master Quiz records: **120**. All 120 have exactly four unique options and unique IDs.

## Source quality and limits

- The reference pages used for these preliminary one-mark answer sets are third-party guide pages. The pages themselves state that the answer material is guide-sourced / not independently verified. Their entries are therefore marked `GUIDE_REFERENCE` or similar; they are not represented as official SCERT answer keys.
- User-supplied reference answers are separately marked `USER_REFERENCE_CROSSCHECK`.
- No textbook PDF SHA-256 match was completed during this batch.
- The existing repository's `questions.md` placement is inconsistent: some files contain sub-lessons belonging to a different Unit folder, and a few sub-lesson files are missing. See [CLASS_08_TAMIL_CONTENT_MAP_2026-11-06.md](./CLASS_08_TAMIL_CONTENT_MAP_2026-11-06.md).
- The current preliminary quiz sets are not yet demonstrated to contain every eligible book-back one-mark item from all nine textbook units. The numeric record counts above are records currently prepared, not a claim of complete book coverage.
- In some units, the draft quiz includes a mix of textbook four-option MCQs and converted one-mark items. These need explicit source-by-source classification before final production.

## Step status

- Step 1: **PARTIAL** — one-mark references have been recorded; full question-by-question coverage and page/source reconciliation remain open. Long / descriptive answer content has not been written; placeholder-only scope retained.
- Step 2: **DRAFTED / PARTIAL** — quiz Markdown created for all nine Units. Original textbook four-option items and converted one-mark items require complete source classification.
- Step 3: **DRAFTED / PARTIAL** — quiz JSON created for all nine Units; three unresolved items excluded from Master.
- Master sync: **DONE FOR CURRENT DRAFT SET** — 120 eligible current records combined into `tamil/book_back_questions/quiz.json`.
- Subject: **NOT COMPLETE** — do not mark Class 8 Tamil complete until source mapping, missing questions, excluded items and full coverage are reconciled.

## Next required work

1. Reconcile the Unit 1 and Unit 2 sub-lesson files against the book's actual sub-lesson boundaries and combined end-of-unit exercises.
2. Locate or extract missing question sets (including தமிழ்மொழி மரபு and any absent sub-lessons) without overwriting the current source files.
3. Restore or correct duplicate options only after checking the textbook page.
4. Compare every generated quiz record with the original question wording and four-option set; classify Step 2 originals separately from Step 3 conversions.
5. Rebuild Unit JSON and Master JSON after the source reconciliation; then rerun QA.
