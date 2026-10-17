# Decision log

Append-only. Add new entries at the bottom. Do not edit earlier entries.

## 2026-10-09 v1

- Reason: First live plan for the owner's Swiss job search. research-report is one reversible task and has no human gate. announcement is a publish graph. Neither fits, so this is a custom graph from the field guide in plans/_template/.
- Change: Added T1 (job-hunter), T2 (searcher), T3 (tailor), T4 (accuracy), M1 (human approval), and T5 (submit). T5 is irreversible, so needs_human is true. Schedule origin is 2026-10-12 09:00 Europe/Zurich. Deadline is 2026-11-09 17:00 Europe/Zurich, four weeks later. Estimates are agent-hours for one pass of about six roles.
- Frozen: none (no task is in progress).

## 2026-10-10 v2

- Reason: The owner asked for one status record of every application. Recorded here before the goal gained that deliverable.
- Change: Added application-tracker to the roster. Added T6, assigned to application-tracker, depending on T5. T6 writes application_status.md from the shortlist, the approval record, and the submission receipts. No running task was rescheduled or reassigned.
- Frozen: none (no task is in progress).

## 2026-10-17 v3

- Reason: The owner asked Applier to fill each application form and to stop before the final submit. Alfonso reviews the filled form and submission happens only after that yes. Recorded here before the goal gained that gate.
- Change: Added applier to the roster (Grok Bot id 8fd043c0-ef1e-4176-98df-1a817ba02a0f). T5 is now Applier filling the form and stopping before submit. Added M2, a needs_human gate where Alfonso reviews the filled form. Added T7, Applier submitting only the forms M2 marks yes. T7 is irreversible, so needs_human is true. T6 now depends on T7. No running task was rescheduled or reassigned.
- Frozen: none (no task is in progress).
