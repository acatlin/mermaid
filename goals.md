``` mermaid

flowchart LR

  %% goals %%

  G[(Goals)] ==> P[(Projects)]
  P --. PT(Tasks)
  PT -->|Is| IC([Incomplete])
  PT -->[Is] ([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
