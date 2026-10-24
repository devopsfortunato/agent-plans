# Gantt

Generated from `plan.yaml` by `python -m planner gantt`. Do not edit by hand.

- Plan: swiss-consulting-2026-10 v1
- Origin: 2026-10-24T09:00:00+02:00
- CPM duration: 26h (std dev 0.9718h along the critical path)
- Resource-constrained makespan: 28h
- Critical path: T2, T4, T5, T6, T9, M2, T10, M3, T11, M4, T12, T13, M5, T14
- `crit` means unconstrained CPM slack is zero. Bar times are the resource-constrained schedule.

| ID | Start | Finish | Slack | Assignee | Critical |
| --- | --- | --- | --- | --- | --- |
| T1 | 0 | 1 | 20 | consulting-tracker | no |
| T2 | 0 | 1 | 0 | consulting-planner | yes |
| T7 | 0 | 3 | 7 | contract-hunter | no |
| T4 | 1 | 5 | 0 | consulting-planner | yes |
| T8 | 1 | 3 | 23 | meetup-scout | no |
| T5 | 5 | 8 | 0 | consulting-planner | yes |
| T3 | 8 | 12 | 9 | consulting-planner | no |
| T6 | 8 | 10 | 0 | accuracy | yes |
| M1 | 12 | 12 | 9 | human | no |
| T9 | 12 | 16 | 0 | consulting-planner | yes |
| M2 | 16 | 16 | 0 | human | yes |
| T10 | 16 | 20 | 0 | consulting-planner | yes |
| M3 | 20 | 20 | 0 | human | yes |
| T11 | 20 | 23 | 0 | consulting-planner | yes |
| M4 | 23 | 23 | 0 | human | yes |
| T12 | 23 | 25 | 0 | consulting-tracker | yes |
| T13 | 25 | 27 | 0 | consulting-planner | yes |
| M5 | 27 | 27 | 0 | human | yes |
| T14 | 27 | 28 | 0 | consulting-planner | yes |

```mermaid
gantt
    title Ticino IT consulting launch v1
    dateFormat YYYY-MM-DD HH:mm
    axisFormat %m-%d %H:%M
    section Setup
    T1 File the migration office record - consulting-tracker :t1, 2026-10-24 09:00, 1h
    T2 File the contract and conflict check - consulting-planner :crit, t2, 2026-10-24 09:00, 1h
    T3 Draft payrolling simulations - consulting-planner :t3, 2026-10-24 17:00, 4h
    M1 Approve payrolling contact - human :milestone, m1, 2026-10-24 21:00, 0m
    section Positioning
    T4 Draft anonymized case studies - consulting-planner :crit, t4, 2026-10-24 10:00, 4h
    T5 Draft the consulting CV - consulting-planner :crit, t5, 2026-10-24 14:00, 3h
    T6 Verify the positioning is anonymized - accuracy :crit, t6, 2026-10-24 17:00, 2h
    section Search
    T7 Search contract roles daily - contract-hunter :t7, 2026-10-24 09:00, 3h
    T8 Scout meetups near Lugano - meetup-scout :t8, 2026-10-24 10:00, 2h
    section Outreach
    T9 Draft broker outreach - consulting-planner :crit, t9, 2026-10-24 21:00, 4h
    M2 Approve broker outreach - human :milestone, crit, m2, 2026-10-25 01:00, 0m
    section Mission
    T10 Draft the first mission - consulting-planner :crit, t10, 2026-10-25 01:00, 4h
    M3 Approve the first mission - human :milestone, crit, m3, 2026-10-25 05:00, 0m
    T11 Draft the Einzelfirma pack - consulting-planner :crit, t11, 2026-10-25 05:00, 3h
    M4 Approve the Einzelfirma - human :milestone, crit, m4, 2026-10-25 08:00, 0m
    section Tracking
    T12 Log outreach and submissions - consulting-tracker :crit, t12, 2026-10-25 08:00, 2h
    T13 Draft due follow-ups - consulting-planner :crit, t13, 2026-10-25 10:00, 2h
    M5 Approve follow-up sends - human :milestone, crit, m5, 2026-10-25 12:00, 0m
    T14 Draft the Monday status - consulting-planner :crit, t14, 2026-10-25 12:00, 1h
```
