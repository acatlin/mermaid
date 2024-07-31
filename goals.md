``` mermaid

flowchart LR

  %% goals %%

  G[(Goals)] ==> P[(Projects)]
  P --> PT(Tasks)

  PT --> C([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
