# எட்டாம் வகுப்பு — தமிழ் பாடம்

இந்த folder-ல் Class 8 தமிழ் பாடத்தின் 9 இயல்களுக்கான Book Back Questions மற்றும் Quiz பணிகள் உள்ளன.

## கட்டாயப் பணி வரிசை

**பொதுவான, அதிகாரப்பூர்வ Step 1–3 விதிகள்:** [`docs/BOOK_BACK_QUIZ_WORKFLOW_TA.md`](../docs/BOOK_BACK_QUIZ_WORKFLOW_TA.md)

ஒவ்வொரு இயலிலும் இதே வரிசையில் செயல்பட வேண்டும்:

1. **STEP 1 — `book_back_questions/answers.md`:** `questions.md`-இல் உள்ள எல்லா கேள்விகளையும் அதே வரிசையில் வைத்தல்; one-mark விடை / விளக்கம் / நேரடி ஆதாரம் சேர்த்தல்; பெரிய வினாக்களுக்கு placeholders மட்டும் பாதுகாத்தல்.
2. **STEP 2 — `book_back_questions/quiz.md`:** பாடநூலில் ஏற்கெனவே நான்கு options உடன் உள்ள அசல் Objective வினாக்களை மட்டும் துல்லியமாகச் சேர்த்தல்.
3. **STEP 3 — `book_back_questions/quiz.md` + `quiz.json`:** மற்ற தகுதியான one-mark / one-word / fill-in / matching / grid வினாக்களை நான்கு-option MCQ-ஆக மாற்றுதல்; படம் இல்லாத image-dependent மற்றும் பெரிய விடை வினாக்களை Quiz-ல் சேர்க்காதல்.

ஒரு இயலின் மூன்று Steps முடிந்து QA செய்த பிறகே அடுத்த இயலுக்குச் செல்லவும். ஒன்பது இயல்களிலும் மூன்று Steps முடிந்து Master Quiz sync சரிபார்த்த பிறகே தமிழ் பாடம் COMPLETE என்று அறிவிக்கவும்.

## Master Quiz நிலை — 2026-11-06

- [Master Quiz JSON](./book_back_questions/quiz.json) — ஒன்பது இயல்களின் Unit JSON-களிலிருந்து ஒத்திசைக்கப்பட்டது.
- தற்போதைய Unit Quiz JSON பதிவுகள்: 123.
- Unit 2 Q4, Unit 9 Q8, Unit 9 Q13 ஆகிய மூன்று extraction பிழைகள் உரிமையாளர் வழங்கிய பாடநூல் திருத்தங்களின்படி சரிசெய்யப்பட்டுள்ளன.
- Master-ல் வெளியிடப்பட்டவை: 123 / 123.
- JSON QA: 123 unique IDs; ஒவ்வொரு பதிவிலும் 4 unique options மற்றும் 0–3 சரியான answer index.
- ஒவ்வொரு Unit-லும் `quiz.md` மற்றும் `quiz.json` எண்ணிக்கை ஒத்திசைந்துள்ளது.
- **நிலை: PARTIAL / DRAFT.** தற்போதைய `questions.md` கோப்புகளின் cross-unit placement மற்றும் முழுக் கேள்வி coverage இன்னும் சரிபார்க்கப்பட வேண்டும். இதை தமிழ் பாடம் COMPLETE என்று கருத வேண்டாம்.
- விவரமான QA: [CLASS_08_TAMIL_BATCH_QA_2026-11-06.md](../docs/CLASS_08_TAMIL_BATCH_QA_2026-11-06.md).

## இயல் கோப்புறைப் பட்டியல்

| இயல் | Folder |
|---|---|
| 1. தமிழ் இன்பம் | [01_tamil_inbam](./01_tamil_inbam/) |
| 2. ஈடில்லா இயற்கை | [02_eedilla_iyarkai](./02_eedilla_iyarkai/) |
| 3. அறிவியல் தொழில்நுட்பம் | [03_arivial_thozhilnutpam](./03_arivial_thozhilnutpam/) |
| 4. கல்வி | [04_kalvi](./04_kalvi/) |
| 5. கலை அழகியல் பண்பாடு | [05_kalai_azhagiyal_panbadu](./05_kalai_azhagiyal_panbadu/) |
| 6. நாகரிகம் தொழில் வணிகம் | [06_nagarigam_thozhil_vanigam](./06_nagarigam_thozhil_vanigam/) |
| 7. நாடு சமூகம் | [07_naadu_samugam](./07_naadu_samugam/) |
| 8. அறம் தத்துவம் சிந்தனை | [08_aram_thathuvam_sinthanai](./08_aram_thathuvam_sinthanai/) |
| 9. மனிதம் ஆளுமை | [09_manitham_aalumai](./09_manitham_aalumai/) |

## இயல் / துணைப்பாடம் கேள்வி கோப்பு இருப்பிடம்

சில துணைப்பாடங்களின் பழைய `questions.md` கோப்புகள் தற்போது வேறு எண்ணுள்ள இயல் folder-களில் இருக்கலாம். அவற்றைத் தவறான இயலுடன் இணைக்காமல் பின்பற்ற வேண்டிய crosswalk: [CLASS_08_TAMIL_CONTENT_MAP_2026-11-06.md](../docs/CLASS_08_TAMIL_CONTENT_MAP_2026-11-06.md). கோப்புகளை நகர்த்துவதற்கு முன் source page, duplicate range, sub-lesson ஆகியவற்றை ஒப்பிடவும்.

## ஒவ்வொரு இயலிலும் பயன்படுத்த வேண்டிய கோப்புகள்

- `book_back_questions/questions.md` — முதன்மை கேள்விப் பட்டியல்; கேள்வி வரிசையின் அடிப்படை.
- `book_back_questions/answers.md` — STEP 1 output.
- `book_back_questions/quiz.md` — STEP 2 + STEP 3 output.
- `book_back_questions/quiz.json` — STEP 3 structured quiz output.

Master Quiz இருப்பின், அதன் path-ஐ [பொது workflow ஆவணத்தின்](../docs/BOOK_BACK_QUIZ_WORKFLOW_TA.md) Master Quiz விதிப்படி sync செய்யவும். தற்போதைய repository layout-ஐ உறுதி செய்யாமல் புதிய Master Quiz path உருவாக்க வேண்டாம்.

**குறிப்பு:** Edition / Medium / Term பற்றிய முடிவு தனியாக [Book Edition Verification Rules](../docs/BOOK_EDITION_VERIFICATION_RULES_TA.md)-இன் படி உறுதிப்படுத்தப்பட வேண்டும்.
