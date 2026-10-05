# My lab evidence / 我的實作紀錄

Use a group code, not real names or student IDs in shared files. / 共用檔只寫組別代碼，不寫姓名或學號。

- Group code / 組別：Not supplied yet
- Tool / 工具：Codex (file work); GitHub web interface (commits)
- Route / 路線：Not supplied yet (individual or paired)
- Tasks completed / 完成題目：A, B (v1 and v2), D
- Material / 素材：NDHU classroom tasks 東華課堂版
- For original-pack work: task number, author/source link and version / 原版實作：N/A
- My role and what I checked / 我的角色與實際檢查：The student reviewed the six Task B v1 scenarios and reported that all passed. The assistant verified all 12 Task A copies against their inputs with SHA-256 hashes, checked that all originals remained, and reviewed the GitHub commit contents. The student has not yet reported a visual retest of the v2 narrow-screen change.

## Scope and plan / 範圍與計畫

Allowed input and output folders / 可讀取與輸出的資料夾：

- A: `practice/01-club-files/input/` → `practice/01-club-files/output/`
- B: `practice/02-campus-picker/activities.json` → `practice/02-campus-picker/output/index.html`
- D: read `practice/04-review/bad-plan.txt`; write `practice/04-review/my-rejection.md`

What I asked for / 原始需求：

- A: organize the 12 fictional inputs into categories, retain duplicates and differing versions, and write a report and manifest.
- B: build one offline HTML activity picker using all six filters/history/language requirements. A later usability refinement added larger, stacked controls on screens 560px wide or narrower.
- D: review the deliberately flawed plan, reject unsafe actions, and propose a safe alternative without executing it.

What I checked before execution / 動手前我檢查了什麼：

- A had 12 inputs and no existing output folder. Identical content pairs were `announcement.txt` / `announcement_copy.txt` and `equipment_list.txt` / `equipment_backup.txt`; `proposal_final.txt` and `proposal_final2.txt` differed.
- B's `activities.json` contained 12 fictional entries. The existing `output` folder was absent.
- D's `bad-plan.txt` explicitly said it was a discussion-only simulation and must not be executed.

## Tests actually performed / 我真的做過的測試

| Test / 測試 | Expected / 預期 | Observed / 實際 | Evidence / 證據 |
|---|---|---|---|
| A: source/copy integrity | Each of the 12 source files has one exact copy; all originals remain. | All 12 output copies matched their input SHA-256 hashes; all 12 originals remained; the manifest contained 12 entries. | Assistant ran the local hash/count check. |
| B v1: six picker scenarios | The six Task B cases behave as specified (including no-match, latest-five history, reset, clear, and English UI). | The student reported “all pass” for the six scenarios. | Student report in chat; no screenshots supplied. |

## One revision / 一次修改

Before / 原來的情況：On narrower screens, filter controls stayed in three columns until the 460px breakpoint.

Request / 我提出的修改：**New requirement** — improve narrow-screen readability and touch use by stacking filters and enlarging labels and controls up to 560px wide.

After and retest / 修改後與重測結果：The v2 commit adds a 560px breakpoint with one-column filters, 0.95rem labels, and 3rem-tall selects. The v2 commit is present on GitHub. A visual retest at 560px or narrower has not been reported yet; no before/after screenshots were supplied.

New requirement or defect? / 新需求還是原規格未做到？New usability requirement; it was not a defect in the original requirements.

## One rejection / 一次退回

Which action I reject and why / 退回哪個動作、為什麼：Rejected organizing all of Downloads, deleting duplicates, treating `final2` as approved, guessing missing values, and publishing automatically. These actions exceed the selected task scope, discard or invent information, and share results without authorization.

An acceptable alternative / 可以怎麼改：Inspect only the selected task folder, preserve originals and all differing versions, report suspected duplicates and unknowns, propose a plan, and wait for review before changes or external sharing.

## Still unverified / 還沒驗證

What I cannot claim is complete / 哪些事不能說已完成：

- Visual check of the v2 layout at 560px or narrower and its affected retest.
- Before/after screenshots for Task B; none were supplied.
- The lab website's self-check ticks/notes and exported `learning-record.md`; the student should complete and export these themselves.
- Group code and whether the work was individual or paired; not supplied.
- The student's own visual comparison of two A source/copy pairs; hash checks passed, but no personal inspection note was supplied.

This is a draft record of known work, not a claim that the remaining evidence has been completed.
