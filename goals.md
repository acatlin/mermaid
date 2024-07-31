``` mermaid

flowchart LR

  %% goals %%

  G[(Goals)] ==> P[(Projects)]
  P --> PT(Tasks)
  PT --x IC([Incomplete])

  PT --> C([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
