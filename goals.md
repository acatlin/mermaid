``` mermaid

flowchart LR
  G(Goals) --> P(Projects)
  P --> PT(Tasks)
  PT -->|Is| IC(Incomplete) & C(Complete)
  C --> R(Review)
  R -->|Creates New| G

```
