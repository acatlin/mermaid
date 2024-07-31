``` mermaid

flowchart LR

  %% goals %%

  G[(Goals)] ==> P[(Projects)]

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
