# Phase 2 Ticket Index

Status: complete
Specification: `PHASE_2_BRAND_ASSET_SYSTEM_SPEC.md`

## Dependency graph

```mermaid
flowchart TD
    P201[P2-01 Production symbol] --> P202[P2-02 Latin wordmark]
    P201 --> P203[P2-03 Arabic wordmark]
    P202 --> P204[P2-04 Bilingual lockup]
    P203 --> P204
    P201 --> P206[P2-06 Preview modifier]
    P201 --> P207[P2-07 Adem family]
    P202 --> P205[P2-05 Usage rules and variants]
    P203 --> P205
    P204 --> P205
    P202 --> P208[P2-08 Manifest freeze]
    P203 --> P208
    P204 --> P208
    P205 --> P208
    P206 --> P208
    P207 --> P208
```

## Work order

| Ticket | Title | Status | Blocked by |
| --- | --- | --- | --- |
| P2-01 | Promote confirmed production symbol | complete | — |
| P2-02 | Finalize Latin wordmark and lockup | complete | P2-01 |
| P2-03 | Finalize Arabic wordmark and lockup | complete | P2-01 |
| P2-04 | Build bilingual lockup | complete | P2-02, P2-03 |
| P2-05 | Complete variants and usage rules | complete | P2-02, P2-03, P2-04 |
| P2-06 | Design Preview modifier | complete | P2-01 |
| P2-07 | Design Adem and Adem Pro marks | complete | P2-01 |
| P2-08 | Freeze manifest and Phase 2 approvals | complete | P2-02–P2-07 |

P2-02, P2-03, P2-06, and P2-07 may proceed independently. P2-04 and P2-05 protect composition consistency; P2-08 is the only Phase 2 exit ticket.
