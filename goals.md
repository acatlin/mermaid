``` mermaid

flowchart LR

  %% goals %%

  G[(Goals)] ==> P[(Projects)]
  P --o PT(Tasks)
  PT --x|Is| IC([Incomplete])
  PT -->[Is] ([Complete])
  C --> R[[Review]]
  R -..->|Creates New| G

```
