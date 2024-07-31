``` mermaid

flowchart LR

  %% Colors %%
  classDef blue fill:#2374f7,stroke:#000,stroke-width:2px,color:#fff
  classDef orange fill:#fc822b,stroke:#000,stroke-width:2px,color:#fff
  classDef green fill:#16b552,stroke:#000,stroke-width:2px,color:#fff
  classDef red fill:#ed2633,stroke:#000,stroke-width:2px,color:#fff
  classDef magenta fill:magenta,stroke:#000,stroke-width:2px,color:#fff

  %% goals %%

  G[(Goals)]:::blue ==> P[(Projects)]:::orange

  P --o |Has| PD(Deadline)
  PD --x |Is| MT(Met):::green
  PD --- |Is| OV(Overdue):::red
  OV --> |Push| FOV{4 Days}:::magenta

  P --> PT(Tasks)


  PT --x IC([Incomplete]):::red

  PT --> C([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
