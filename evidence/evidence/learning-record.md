# Learning record | Let AI help with a small campus task

Route: Two periods / 100 minutes
Exported: 10/5/2026, 4:06:01 PM

> This is the downloaded site record with a working evidence summary added locally. It is not proof that an agent executed anything, and it does not update the learning site. Add your own files, screenshots and test evidence before treating a check as complete.

## Setup — Before you start
- [x] I can state the full path of the task folder I selected
- [ ] My partner and I checked the tool's current permission and approval settings
- [x] The practice folder contains no real names, student IDs, grades, private photos or passwords

**Notes:**
Task folders in this workspace: `practice/01-club-files/`, `practice/02-campus-picker/`, and `practice/04-review/`. Route: individual. No group code was assigned. Permission/approval settings were not recorded here. The partner-specific check below does not apply to this individual route.

**Actual evidence (add your own):**
Workspace/task-folder path: `C:\Users\LOQ\Documents\Agent\agent-lab-w05-main\agent-lab-w05-main\practice\01-club-files` (and the B and D folders are under the same `practice` directory). No setup screenshots or permission-setting evidence are included in this folder.

## Task A — One task card to organize a folder
- [x] All originals remain and each organized copy maps to a source (12 for NDHU; actual inventory for the original pack)
- [x] Similarly named files with differing contents were all kept
- [x] I compared two original/copy pairs by content, not only by filename
- [ ] My partner can find unresolved decisions in the organization report

**Notes:**
The 12 source files and categorized output copies are present. The assistant verified all 12 manifest source/destination pairs by SHA-256; every pair matched, and all originals remain. Both differing proposal versions are retained. The content-comparison screenshot's editor tabs truncate filenames, but the hash log verifies the pairs independently.

**Actual evidence (add your own):**
Files: `practice/01-club-files/output/report.md`, `practice/01-club-files/output/manifest.json`, and files under `practice/01-club-files/output/{communications,planning,resources}/`. `evidence/evidence/a-copy-verification.txt` records SHA-256 matches for all 12 manifest pairs. `screenshots/Screenshot 2026-10-06 221907.png` shows 12 input items and the categorized output with three folders, manifest, and report. `screenshots/A-announcement-content-comparison.png` shows matching text in four editor windows, though the filenames are truncated.

## Task B — Build “What can I do between classes?”
- [x] Indoor / 15 / low returns only A01–A04
- [x] Outdoor / 15 / medium shows no matches and does not relax the filters
- [x] Outdoor / 30 / medium returns A09 every time
- [ ] All / 60 / all, six successful picks: only the latest five remain, newest first
- [x] Reset returns all / 30 / all and the history remains
- [x] After clearing history and switching to English, history is empty and all controls and activity names are in English
- [ ] I made one revision, retested the affected functions and kept before/after evidence

**Notes:**
`practice/02-campus-picker/output/index.html` is present. Screenshots show no matches for Outdoor / 15 / Medium, A09 for Outdoor / 30 / Medium, Indoor / 15 / Low with only A01–A04 in the result/history, English and Chinese interfaces with five visible recent picks, All / 30 / All with history still visible, English mode with cleared history, and the stacked narrow layout at a 400px viewport. The screenshots still do not establish six successful picks before history was limited to five, nor a same-width before/after comparison for the revision.

**Actual evidence (add your own):**
File: `practice/02-campus-picker/output/index.html`. Screenshots: `screenshots/Screenshot 2026-10-06 221518.png` (Outdoor / 15 / Medium, no matches); `screenshots/Screenshot 2026-10-06 221531.png` (Outdoor / 30 / Medium, A09); `screenshots/B-indoor-15-low.png` (Indoor / 15 / Low, only A01–A04 appear); `screenshots/Screenshot 2026-10-06 221627.png` (Chinese interface and five visible history entries); `screenshots/Screenshot 2026-10-06 221634.png` (English interface and five visible history entries); `screenshots/Screenshot 2026-10-06 221749.png` (narrow layout; width not shown); `screenshots/Screenshot 2026-10-06 224316.png` (Outdoor / 15 / Low, A07); `screenshots/Screenshot 2026-10-06 224352.png` (Outdoor / 60 / Medium with five history entries); `screenshots/Screenshot 2026-10-06 224427.png` (All / 30 / All with five history entries); `screenshots/Screenshot 2026-10-06 224438.png` (English interface and activity name with empty history); `screenshots/Screenshot 2026-10-06 224518.png` (stacked layout at 400px). Six picks followed by the latest-five result and a same-width before/after comparison are still unverified.

## Task C — clean equipment records
- [x] 10 input rows become 9 valid rows and the removed count is reported
- [x] Rows sharing item_id are all kept, not merged or deleted
- [x] Missing and negative quantities are flagged, not replaced with zero or made positive

**Notes:**
The cleaned output retains nine nonempty records and reports one removed blank row. Duplicate IDs EQ01 and EQ02 are retained. The missing quantity in row 7 and negative quantity in row 8 remain unchanged and are flagged.

**Actual evidence (add your own):**
Input: `practice/03-equipment/equipment.json`; outputs: `practice/03-equipment/output/cleaned-equipment.json` and `practice/03-equipment/output/report.md`. The output was parsed and checked for row count, removed count, duplicate-ID retention, original flagged quantity values, and flags. Screenshots: `screenshots/C-equipment-cleaning-report.png`, `screenshots/C-cleaned-json-summary.png`, `screenshots/C-cleaned-json-records.png`, `screenshots/C-cleaned-json-duplicates-and-missing-quantity.png`, and `screenshots/C-cleaned-json-negative-quantity.png`.

## Task D — Would you approve this plan?
- [x] I identified at least two problems and explained why they are unacceptable
- [x] I wrote a rejection that proposes an allowed alternative

**Notes:**
The written rejection is present and addresses several unsafe actions with an allowed alternative. The file itself is evidence of the written response; no separate test or screenshot is needed unless required by the course site.

**Actual evidence (add your own):**
File: `practice/04-review/my-rejection.md`. It rejects broad-scope file changes, duplicate deletion, assumptions about `final2`, invented values, and automatic publication, and proposes a scoped review-first alternative.

