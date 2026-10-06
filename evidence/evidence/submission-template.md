# My lab evidence / 我的實作紀錄

Use a group code, not real names or student IDs in shared files. / 共用檔只寫組別代碼，不寫姓名或學號。

- Group code / 組別：N/A — no group code assigned; individual work.
- Tool / 工具：Codex; GitHub web interface is listed in the draft, but the commits still need to be checked on your repository page.
- Route / 路線：Individual 個人
- Tasks completed / 完成題目：A, B (v1 and revision), C, D.
- Material / 素材：NDHU classroom tasks 東華課堂版
- For original-pack work: task number, author/source link and version / 原版實作：N/A
- My role and what I checked / 我的角色與實際檢查：I supplied screenshots showing the A input/output folders and announcement text, and the B no-match result, A09 result, English/Chinese screens with five visible history entries, and a narrow stacked layout. The assistant verified all 12 A source/copy pairs by SHA-256; the log is saved in `evidence/evidence/a-copy-verification.txt`. The screenshots do not establish every required B test. GitHub commit history is not available in this workspace, so commit status still needs checking on the repository page.

## Scope and plan / 範圍與計畫

Allowed input and output folders / 可讀取與輸出的資料夾：

- A: `practice/01-club-files/input/` → `practice/01-club-files/output/`
- B: `practice/02-campus-picker/activities.json` → `practice/02-campus-picker/output/index.html`
- C: `practice/03-equipment/equipment.json` → `practice/03-equipment/output/`
- D: read `practice/04-review/bad-plan.txt`; write `practice/04-review/my-rejection.md`

What I asked for / 原始需求：

- A: organize the 12 fictional inputs into categories, retain duplicates and differing versions, and write a report and manifest.
- B: build one offline HTML activity picker using the location, time, energy, history, reset, and language requirements. A later usability request asked for larger, stacked controls on screens 560px wide or narrower.
- D: review the deliberately flawed plan, reject unsafe actions, and propose an allowed alternative without executing the plan.
- C: remove only the empty row, retain records with repeated IDs, and flag missing or negative quantities without changing them.

What I checked before execution / 動手前我檢查了什麼：

- A: the input folder contains 12 files; the output contains communications, planning, and resources folders, a manifest, and a report. The report identifies suspected identical pairs and differing proposal versions.
- B: `activities.json` and `output/index.html` are present.
- D: `bad-plan.txt` is a simulated plan; `my-rejection.md` contains a written rejection and alternative.
- C: the input contains 10 rows, including one empty object, duplicate IDs, a missing quantity, and a negative quantity.

## Tests actually performed / 我真的做過的測試

| Test / 測試 | Expected / 預期 | Observed / 實際 | Evidence / 證據 |
|---|---|---|---|
| A: organization and content comparison | Keep all originals and make one organized copy per input; compare two source/copy pairs by content. | All 12 manifest source/destination pairs exist and have matching SHA-256 hashes. The differing proposal versions are both retained. | `evidence/evidence/a-copy-verification.txt`; `evidence/evidence/screenshots/Screenshot 2026-10-06 221907.png`; `evidence/evidence/screenshots/A-announcement-content-comparison.png`; `practice/01-club-files/output/manifest.json`; `practice/01-club-files/output/report.md` |
| B: picker scenarios shown in screenshots | Indoor / 15 / Low returns only A01–A04; no matches for Outdoor / 15 / Medium; A09 for Outdoor / 30 / Medium; Reset preserves history; cleared history and English UI. | Screenshots show the required Indoor / 15 / Low items, the no-match result, A09, All / 30 / All with five history entries, and English UI with empty history. Six picks followed by a five-item history are not established. | `evidence/evidence/screenshots/B-indoor-15-low.png`; `evidence/evidence/screenshots/Screenshot 2026-10-06 221518.png`; `evidence/evidence/screenshots/Screenshot 2026-10-06 221531.png`; `evidence/evidence/screenshots/Screenshot 2026-10-06 224427.png`; `evidence/evidence/screenshots/Screenshot 2026-10-06 224438.png` |
| C: equipment cleanup | 10 input rows become 9 output records; report 1 removed row; preserve duplicate IDs; flag missing and negative quantities without changing them. | Output has 9 records; empty source row 6 is the only removed row; duplicate EQ01 and EQ02 records remain; row 7's empty quantity and row 8's -1 remain and are flagged. | `practice/03-equipment/output/cleaned-equipment.json`; `practice/03-equipment/output/report.md`; `evidence/evidence/screenshots/C-equipment-cleaning-report.png`; `evidence/evidence/screenshots/C-cleaned-json-summary.png`; `evidence/evidence/screenshots/C-cleaned-json-records.png`; `evidence/evidence/screenshots/C-cleaned-json-duplicates-and-missing-quantity.png`; `evidence/evidence/screenshots/C-cleaned-json-negative-quantity.png` |

## One revision / 一次修改

Before / 原來的情況：The draft describes the earlier layout as keeping filters in three columns until a 460px breakpoint. A before screenshot at the same viewport width is not available here.

Request / 我提出的修改：**New usability requirement** — improve narrow-screen readability and touch use by stacking filters and enlarging labels and controls up to 560px wide.

After and retest / 修改後與重測結果：A screenshot shows stacked controls at a 400px viewport. This verifies the current narrow layout. A same-width before/after comparison is not available, so the full before/after evidence check remains incomplete. The v2 GitHub commit is reported in the earlier draft but has not been verified from this workspace.

New requirement or defect? / 新需求還是原規格未做到？New usability requirement, according to the earlier draft; it was not described as a defect in the original requirements.

## One rejection / 一次退回

Which action I reject and why / 退回哪個動作、為什麼：The written rejection refuses organizing all of Downloads, deleting duplicates, treating `final2` as approved, guessing missing values, and publishing automatically. These actions exceed the selected scope, discard or invent information, or share results without approval.

An acceptable alternative / 可以怎麼改：Inspect only the selected task folder, preserve originals and differing versions, report suspected duplicates and unknowns, propose a plan, and wait for review before changes or external sharing.

Evidence / 證據：`practice/04-review/my-rejection.md`

## Still unverified / 還沒驗證

What I cannot claim is complete / 哪些事不能說已完成：

- Complete the remaining B checks: six successful picks leaving only the newest five; and a same-width before/after comparison for the narrow-screen revision.
- The A comparison screenshot truncates filenames, but the SHA-256 log verifies all 12 source/copy pairs.
- A same-width before/after screenshot for the B revision is not available.
- The learning-site self-checks and notes have not been completed/exported based on the current local record.
- Required GitHub commits and final evidence commit have not been verified from this workspace. Check the repository page and confirm the final commit includes `evidence/`, the exported `learning-record.md`, screenshots, and this filled template.

This record summarizes available files and screenshots; it does not claim unverified tests or commits are complete.
