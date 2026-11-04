# SCERT Class 8 Textbook Edition Verification Audit Report (28 Records)

**Audit Execution Environment:** GitHub Actions Runner (Ubuntu 22.04 LTS)  
**Execution Timestamp:** 2026-11-04T13:41:16.586975+00:00 UTC  
**Target Repository:** Eaglesiva/tn-class-08  
**Target Branch:** scert/class-08/audit-2026-27  
**Live Official API URL:** `https://emis3.tnschools.gov.in/api/get_scert_books`  
**Raw API Snapshot SHA-256:** `404f283443b1f7a6a0fae814092aae556d0419ad2b4b2c0b0a0f7ebd756cc3e4`  

---

## 1. Class-Wide Metric Reconciliation Table (28 Records Complete)

| No. | Audit Verification Metric | Count | Reconciliation & Evidence Details |
|---|---|:---:|---|
| 1 | **Total Class 8 Official API Records** | **28** | Complete live API inventory across all sections: 25 academic, 1 valuation module, 2 physical education resource books. |
| 2 | **In-Scope Records (State Board Tamil & English)** | **8** | Core State Board academic books: Tamil, English, Mathematics (TM/EM), Science (TM/EM), Social Science (TM/EM). All full-year standalone textbooks. |
| 3 | **Out-of-Scope Records** | **20** | • 9 Minority language mediums (Telugu, Malayalam, Urdu for Maths, Science, Social)<br>• 8 Minority/optional language readers (Telugu, Kannada, Malayalam, Urdu, Hindi, Sanskrit, Arabic, French)<br>• 1 Value education supplementary module (`8th_Std_Value_Education_Module.pdf`)<br>• 2 Physical education teacher's resource books (Tamil & English) |
| 4 | **Official URLs Successfully Downloaded & Audited** | **8** | All 8 in-scope State Board books sequentially downloaded to runner `/tmp/`, verified, and removed. 100% available on CDN. |
| 5 | **Official URLs Returning HTTP 403 on GET** | **0** | Zero in-scope books returned 403. All 8 core State Board textbooks are accessible on CloudFront CDN. |
| 6 | **Books Matching Existing Local Baseline** | **0** | Zero. Baseline folders contain legacy 2018/2019/2022 separate book splits. |
| 7 | **Books with Confirmed New/Different Edition (2026)** | **8** | All 8 downloaded books confirmed as 2026 curriculum volumes with differing text/pages and 2023/2024 reprint imprints. |
| 8 | **Books Successfully Split & Validated into 1-Page PDFs** | **8** | All confirmed new edition books split into individual pages with 100% passing structural validation (magic bytes, 1-page, renderable, size, continuity). |
| 9 | **Books Ingested into Audit Branch Editions** | **8** | Ingested under immutable paths in `official_editions/2026-27/full_year/`. |
| 10 | **Books Requiring Manual Review (TOC boundaries)** | **0** | Zero. All 8 books in Class 8 are standalone single-subject textbooks (`SINGLE_SUBJECT_STANDALONE`). |
| 11 | **Books Currently Inaccessible on CDN (HTTP 403)** | **0** | Zero in-scope books. |
| 12 | **Books Not Checked** | **0** | Every single one of the 28 records was evaluated and cataloged. |

---

## 2. Git Safety & Production Protection
- **Main Branch:** Completely protected. Zero changes to existing production folders (`tamil/`, `english/`, `maths_tm/`, `maths_em/`, `science_tm/`, `science_em/`, `social_science_tm/`, `social_science_em/`, `index.html`, `viewer.html`).
- **Audit Branch:** All files stored strictly under `official_editions/2026-27/` and root audit manifests on `scert/class-08/audit-2026-27`.
- **Master PDFs:** Zero master PDFs committed to Git. Downloaded strictly to runner temporary `/tmp/` and removed immediately after splitting.
