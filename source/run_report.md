# Handwheel V8 A-F Luna Max grading run

- Model: `gpt-5.6-luna` with `model_reasoning_effort=max`.
- Transport: Codex CLI (`codex exec`); no direct SDK/API call.
- Dataset: `C:\CAD_Research\projects\07_2026-08-05_Synthetic_Image_Only_CAD_VQA\data\benchcad\models\handwheel_000480_s4420\vqa_v8_af`; six labeled choices A-F and four V8 images/question.
- The question stems and original correct answers are unchanged; two additional distractors were appended.
- The model was instructed to return both the selected letter and exact choice text.
- Completed: **10/10**; correct: **10/10** (100.0%).
- Difficulty-weighted score: **40/40**.
- Ground-truth answer labels: A=3, B=3, C=2, D=2, E=0, F=0.

## Per-question results

| # | QA ID | Predicted label | Predicted text | Ground truth label | Status |
|---:|---|---|---|---|---|
| 1 | `handwheel_000480_s4420_v3_axis_component_bundle` | A | the wheel axle is X, the rim lies in YZ, the handgrip is on +Y and +X, and the short hub extension is on -X | A | CORRECT |
| 2 | `handwheel_000480_s4420_v3_symmetry_restoration` | B | the long handgrip | B | CORRECT |
| 3 | `handwheel_000480_s4420_v3_coaxial_offset_profile` | C | the short hub extension shares the central X axis while the handgrip is parallel to X but radially offset | C | CORRECT |
| 4 | `handwheel_000480_s4420_v3_spoke_grip_registration` | D | at the outer rim along the continuation of one spoke | D | CORRECT |
| 5 | `handwheel_000480_s4420_v3_bounded_sector_topology` | A | five open sectors enclosed by one continuous rim with flat radial bars | A | CORRECT |
| 6 | `handwheel_000480_s4420_v3_through_opening_axial_visibility` | B | it is one continuous opening visible from both signed X sides | B | CORRECT |
| 7 | `handwheel_000480_s4420_v3_negative_x_depth_chain` | C | short hub extension, wheel rim, long handgrip | C | CORRECT |
| 8 | `handwheel_000480_s4420_v3_one_spoke_step_transform` | D | the wheel and central hub repeat but the handgrip moves to a sector with no handgrip | D | CORRECT |
| 9 | `handwheel_000480_s4420_v3_yz_reflection_counterfactual` | A | the +X handgrip would lie on -X while the short hub extension would lie on +X | A | CORRECT |
| 10 | `handwheel_000480_s4420_v3_parallel_axis_correspondence` | B | the central opening axis and the long handgrip axis are both X, although only the central opening is on-axis | B | CORRECT |

Raw prompts, CLI logs, and isolated four-image staging folders are retained beside this report.
