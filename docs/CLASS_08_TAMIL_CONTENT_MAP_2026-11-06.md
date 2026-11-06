# Class 8 Tamil — Unit / Sub-lesson / Question File Crosswalk

- Audit date: 2026-11-06
- Scope: Tamil textbook Unit 1 and Unit 2 question-file placement
- Repository: https://github.com/Eaglesiva/tn-class-08

## Confirmed textbook hierarchy

Unit 1: **தமிழ் இன்பம்**

1. 1.1 தமிழ்மொழி வாழ்த்து
2. 1.2 தமிழ்மொழி மரபு
3. 1.3 தமிழ் வரிவடிவ வளர்ச்சி
4. 1.4 சொற்பூங்கா
5. 1.5 எழுத்துகளின் பிறப்பு

Unit 2: **ஈடில்லா இயற்கை**

1. 2.1 ஓடை
2. 2.2 கோணக்காத்துப் பாட்டு
3. 2.3 நிலம் பொது
4. 2.4 வெட்டுக்கிளியும் சருகுமானும்
5. 2.5 வினைமுற்று
6. 2.6 திருக்குறள்

Cross-check references:
- https://mytamil.in/pdf/tb/8.php — chapter-by-chapter listing, including Units 1 and 2.
- https://www.brainkart.in/article/Poem--Tamil-mozhi-marabu--Questions-and-Answers_11405/ — explicitly labels தமிழ்மொழி மரபு as a poem inside இயல் 1: தமிழ் இன்பம்.
- https://tnquestionpapers.com/8th-tamil.php — lists the same Unit 1 and Unit 2 sub-lesson groups.
- Repository owner confirmation in this conversation (2026-11-06).

## Current repository question-file evidence

| Textbook sub-lesson | Current question file found | Finding |
|---|---|---|
| 1.1 தமிழ்மொழி வாழ்த்து | `tamil/01_tamil_inbam/book_back_questions/questions.md` | Correct content; first poem. |
| 1.2 தமிழ்மொழி மரபு | No separate matching `questions.md` found in the nine inspected unit folders | Question extraction coverage gap. Do not mark the whole Unit 1 Step 1 complete yet. |
| 1.3 தமிழ் வரிவடிவ வளர்ச்சி | `tamil/03_arivial_thozhilnutpam/book_back_questions/questions.md` | File title and its own note say it was extracted from old `01_tamil_inbam`, pages 18–22. It belongs to Unit 1, not the Unit 3 folder label. |
| 1.4 சொற்பூங்கா | No clearly named standalone `questions.md` found | The current Unit 2 root file begins with one-letter-word activities; whether these are the complete 1.4 set needs source-page reconciliation. |
| 1.5 எழுத்துகளின் பிறப்பு | `tamil/05_kalai_azhagiyal_panbadu/book_back_questions/questions.md` | File title says எழுத்துகளின் பிறப்பு; its content contains an explicit note that the combined end-of-unit exercise covers all of Iyal 1. It is Unit 1 content, not the Unit 5 folder label. |
| 2.1 ஓடை | `tamil/06_nagarigam_thozhil_vanigam/book_back_questions/questions.md` | File note says it was extracted from old `02_eedilla_iyarkai`, pages 33–36. It belongs to Unit 2, not the Unit 6 folder label. |
| 2.2 கோணக்காத்துப் பாட்டு | `tamil/07_naadu_samugam/book_back_questions/questions.md` | File note says it was extracted from old `02_eedilla_iyarkai`, pages 37–39. It belongs to Unit 2, not the Unit 7 folder label. |
| Unit 2 combined question set | `tamil/02_eedilla_iyarkai/book_back_questions/questions.md` | Large combined file. It contains Unit 1 spillover / grammar content before the Unit 2 material and overlaps with the separate 2.1 / 2.2 files. Deduplication and section boundaries need checking before quiz/master sync. |

## Execution implications

1. The earlier assumption that every root folder's `questions.md` necessarily belongs to the folder's Unit title is unsafe.
2. The Unit 1 question set is currently distributed across folders 01, 03 and 05, while at least one Unit 1 sub-lesson (1.2) has no separate matching question file in the inspected tree.
3. The Unit 2 question set is currently distributed across folders 02, 06 and 07, with likely overlap between the combined file and the two sub-lesson extracts.
4. Preserve every existing source file. Do not delete, overwrite, move or merge question files until each source page and duplicate range has been reconciled.
5. Create Answers / Quiz against the exact verified question set for each sub-lesson. Do not treat a misplaced question file as evidence that the corresponding numbered Unit is complete.
6. The resolved Unit-title / poem-title clarification is not an edition blocker. These are repository organization and question-coverage checks.

## Current work status

- Unit 1.1 தமிழ்மொழி வாழ்த்து: Step 1 started in `tamil/01_tamil_inbam/book_back_questions/answers.md`; Q4 in the current source file is flagged `REVIEW_REQUIRED` because the stem and options conflict with multiple answer references.
- Unit 1 overall: not complete. Other sub-lesson question coverage and placement still need reconciliation.
- Unit 2 overall: not started.
- Steps 2 and 3 must remain in order after Step 1 is complete for the relevant verified sub-lesson set.
