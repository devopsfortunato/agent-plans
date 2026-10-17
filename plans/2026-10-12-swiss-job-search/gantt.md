# Gantt

Generated from `plan.yaml` by `python -m planner gantt`. Do not edit by hand.

- Plan: swiss-job-search-2026-10 v3
- Origin: 2026-10-12T09:00:00+02:00
- CPM duration: 39h (std dev 2.8916h along the critical path)
- Resource-constrained makespan: 39h
- Critical path: T1, T2, T3, T4, M1, T5, M2, T7, T6
- `crit` means unconstrained CPM slack is zero. Bar times are the resource-constrained schedule.

| ID | Start | Finish | Slack | Assignee | Critical |
| --- | --- | --- | --- | --- | --- |
| T1 | 0 | 7 | 0 | job-hunter | yes |
| T2 | 7 | 16 | 0 | searcher | yes |
| T3 | 16 | 28 | 0 | tailor | yes |
| T4 | 28 | 32 | 0 | accuracy | yes |
| M1 | 32 | 32 | 0 | human | yes |
| T5 | 32 | 36 | 0 | applier | yes |
| M2 | 36 | 36 | 0 | human | yes |
| T7 | 36 | 38 | 0 | applier | yes |
| T6 | 38 | 39 | 0 | application-tracker | yes |

```mermaid
gantt
    title Swiss DevSecOps job search v3
    dateFormat YYYY-MM-DD HH:mm
    axisFormat %m-%d %H:%M
    section Search
    T1 Find matching Swiss roles - job-hunter :crit, t1, 2026-10-12 09:00, 7h
    section Research
    T2 Research each company - searcher :crit, t2, 2026-10-12 16:00, 9h
    section Applications
    T3 Tailor CV and cover letter - tailor :crit, t3, 2026-10-13 01:00, 12h
    section Review
    T4 Verify CV matches the posting - accuracy :crit, t4, 2026-10-13 13:00, 4h
    section Gate
    M1 Approve applications - human :milestone, crit, m1, 2026-10-13 17:00, 0m
    T5 Fill application forms - applier :crit, t5, 2026-10-13 17:00, 4h
    M2 Approve filled forms - human :milestone, crit, m2, 2026-10-13 21:00, 0m
    T7 Submit approved applications - applier :crit, t7, 2026-10-13 21:00, 2h
    section Tracking
    T6 Log application status - application-tracker :crit, t6, 2026-10-13 23:00, 1h
```
