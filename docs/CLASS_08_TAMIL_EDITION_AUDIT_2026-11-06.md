# Class 8 Tamil — Book Edition Verification Audit

- Audit date: 2026-11-06
- Class: 8
- Subject: Tamil
- Medium: Tamil (repository page set appears Tamil medium; exact cover/imprint not yet verified)
- Term / volume: Repository contains a consolidated annual page set (`tamil/pages.json` maps pages 11–232 across 9 lesson folders); current official 2026–27 Class 8 Tamil PDF not directly opened/verified.
- Repository source: https://github.com/Eaglesiva/tn-class-08
- Existing local pages: `tamil/01_tamil_inbam/page_011.pdf` onward; PDF bytes and imprint were not inspected in this audit.
- Existing question source: `tamil/01_tamil_inbam/book_back_questions/questions.md`
- Existing source references in questions.md: local Windows `file:///e:/...` HTML path only; not a durable public source URL.

## Evidence reviewed

1. Government of Tamil Nadu / Tamil Nadu Textbook and Educational Services Corporation official website:
   https://www.textbookcorp.in/
   The website announces that Class 8 annual textbooks for academic year 2026–27 went on sale from 14-05-2026. This verifies that the new academic-year Class 8 annual textbook release exists, but the page does not expose a direct Class 8 Tamil PDF, exact edition/imprint, or lesson list.
2. NDLI Standard VIII collection:
   https://www.ndl.iitkgp.ac.in/se_document/tn_school_board/12345678_tnbrd/16130
   Lists Class 8 Tamil/English Term I, Term II and Term III volumes. The opened Standard VIII collection confirms Department of School Education, Government of Tamil Nadu as content provider.
3. NDLI item:
   https://www.ndl.iitkgp.ac.in/se_document/tn_school_board/12345678_tnbrd/25434
   Item metadata describes a combined Tamil/English Term I Volume I book, 8 pages, publisher Tamil Nadu Textbook and Educational Services Corporation, publisher date 2012-01-01. This is historical evidence, not proof of the currently prescribed edition.
4. Third-party listing:
   https://tnkalvi.online/textbooks/book/class-8-tm-full-year-tamil
   Lists a full-year Class 8 Tamil PDF with filename `Class_8_Tamil_2025_Edition-www.tntextbooks.in.pdf` hosted through Google Drive. Third-party source, not an official Government-hosted file; not sufficient to establish current validity.
5. Third-party listing:
   https://ekalvi.in/class-8/class-8-tamil-tm-pdf/
   Describes a 2024–25 full-year Class 8 Tamil edition and a syllabus sequence different from the repository's current lesson segmentation. Third-party source.

## Comparison / finding

- Existing repository `questions.md` title for its first lesson is `01 தமிழ்மொழி வாழ்த்து` and its note maps the content to pages 11–14.
- Public third-party 2024–25 listing describes a full-year textbook whose first unit is `இன்பத்தமிழ்` and provides a different structure.
- The above mismatch suggests the repository's nine-lesson mapping / question extraction may represent a different book structure or an earlier source extraction. It must not be assumed to match the 2026–27 prescribed edition.
- No file-level SHA-256 comparison with an official 2026–27 PDF was possible.
- No official 2026–27 Tamil book cover, imprint, contents pages, or Book Back pages were directly inspected in this audit.

## Decision

**CURRENT_VALIDITY_UNVERIFIED**

Reason: Official 2026–27 Class 8 annual textbook release is confirmed, but the exact Tamil PDF and its contents were not directly accessible for page-level and file-level comparison. Existing repository pages/questions must be preserved. Do not publish final answers or quizzes against a presumed edition until the exact intended book is verified.

## Next required evidence

- Obtain the official 2026–27 Class 8 Tamil-medium annual PDF from the school / official SCERT or Textbook Corporation distribution channel.
- Inspect cover, imprint, contents and each Book Back page.
- Compare first and last pages and all nine lesson groups against the repository page set.
- Record SHA-256 of official PDF and repository source PDF if both are available.
- Only then start Step 1 answers for the verified edition.
