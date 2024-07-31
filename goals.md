``` mermaid

flowchart LR

  %% Colors %%
  classDef blue fill:#2374f7,stroke:#000,stroke-width:2px,color:#fff

  %% goals %%

  G[(Goals)]:::blue ==> P[(Projects)]

  P --o |Has| PD(Deadline)
  PD --x |Is| MT(Met)
  PD --- |Is| OV(Overdue)
  OV --> |Push| FOV{4 Days}

  P --> PT(Tasks)


  PT --x IC([Incomplete])

  PT --> C([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
