# Handwheel V9 A-F Luna Max grading run

- Model: `gpt-5.6-luna` with `model_reasoning_effort=max`.
- Transport: Codex CLI (`codex exec`); no direct SDK/API call.
- Dataset: `C:\CAD_Research\projects\07_2026-08-05_Synthetic_Image_Only_CAD_VQA\data\benchcad\models\handwheel_000480_s4420\vqa_v9_af`; six labeled choices A-F and four V9 images/question.
- The question stems and original correct answers are unchanged; two additional distractors were appended.
- The model was instructed to return both the selected letter and exact choice text.
- Completed: **10/10**; correct: **10/10** (100.0%).
- Difficulty-weighted score: **40/40**.
- Ground-truth answer labels: A=2, B=2, C=2, D=2, E=1, F=1.

## Per-question results

| # | QA ID | Predicted label | Predicted text | Ground truth label | Status |
|---:|---|---|---|---|---|
| 1 | `handwheel_000480_s4420_v9_appendage_face_relation` | A | the long handgrip attaches at the rim along one spoke and projects from one face, while the short hub extension is centered and projects from the opposite face | A | CORRECT |
| 2 | `handwheel_000480_s4420_v9_repeat_breaker` | B | the long handgrip | B | CORRECT |
| 3 | `handwheel_000480_s4420_v9_centered_vs_offset` | C | the short hub extension follows the opening's center, while the long handgrip runs in the same front-to-back direction but is displaced toward the rim | C | CORRECT |
| 4 | `handwheel_000480_s4420_v9_grip_spoke_registration` | D | it continues the line of one spoke at the rim | D | CORRECT |
| 5 | `handwheel_000480_s4420_v9_sector_boundary_pattern` | E | five open sectors separated by flat bars and enclosed by one continuous rim | E | CORRECT |
| 6 | `handwheel_000480_s4420_v9_opening_continuity` | F | it is one continuous opening that can be seen from both ends | F | CORRECT |
| 7 | `handwheel_000480_s4420_v9_end_to_end_depth_order` | A | short hub extension, wheel rim, long handgrip | A | CORRECT |
| 8 | `handwheel_000480_s4420_v9_one_spoke_shift` | B | the repeated wheel pattern would coincide but the long handgrip would move to a different sector | B | CORRECT |
| 9 | `handwheel_000480_s4420_v9_front_back_swap` | C | the long handgrip and the short hub extension | C | CORRECT |
| 10 | `handwheel_000480_s4420_v9_shared_depth_direction` | D | both extend in the same front-to-back direction, but only the opening is centered and the handgrip is offset toward the rim | D | CORRECT |

Raw prompts, CLI logs, and isolated four-image staging folders are retained beside this report.
