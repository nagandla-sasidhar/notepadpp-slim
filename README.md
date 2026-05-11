# SLIM Language — Notepad++ User Defined Language

Syntax highlighting and code folding for `.slm` files in Notepad++.

## Install

1. Open **Notepad++**
2. Go to **Language** → **User Defined Language** → **Define Your Language...**
3. Click **Import...** in the bottom-left
4. Select `slim.udl.xml` from this folder
5. Click **OK** and **restart Notepad++**
6. Open any `.slm` file — highlighting applies automatically

## Colour Scheme (VS Code Dark+ inspired)

| Construct | Colour |
|---|---|
| `@key`, `@+key` — sigils | Teal (#1B7F79) |
| `CALL ASSERT YIELD …` — directives | Yellow (#DCDCAA) |
| Reserved header keys | Blue (#569CD6) |
| Type names (`str`, `int` …) | Teal (#4EC9B0) |
| `=== BLOCK` / `=== /BLOCK` | Purple (#C586C0) |
| `~ comment` | Green italic (#6A9955) |
| Numbers | Light green (#B5CEA8) |

## Code Folding

Notepad++ will fold `=== BLOCK … === /BLOCK` regions. Use the margin arrows or:
- **Fold all**: View → Fold All
- **Unfold all**: View → Unfold All

## Notes

- Notepad++ UDL does not support regex-based per-token colouring, so `$var` inline
  highlighting is not available (use the VSCode or IntelliJ plugin for full highlighting).
- To associate `.slm` extension permanently: go to Settings → Style Configurator,
  select **SLIM** language and add `slm` to the file extension list.
