# Intellij Platform

# Action
- IdeaVim uses `AnAction` for each vim-command.
- `#update` method can use `e.getPresentation().setEnabledAndVisible(...)` to 

## Action XML
- There exists an `<action>` tag that goes in `plugin.xml`
- It seems like IdeaVim doesn't use it for much

# Editor
- 

## Caret Model
- Exists `Offset`, `VisualPosition`, `LogicalPosition`

### Logical Position
- 0-indexed (line, col)
- Ignores code folding, soft line wrap

### Caret Lean
Caret can be associated with preceding or succeeding character

