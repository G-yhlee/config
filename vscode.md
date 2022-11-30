```json
// Place your key bindings in this file to override the defaults
// extension :: cnt + shift + d
[
  {
    "key": "shift+r",
    "command": "keybindings.editor.resetKeybinding"
  },
  {
    "key": "alt+/",
    "command": "workbench.action.terminal.toggleTerminal"
  },
  {
    "key": "ctrl+`",
    "command": "-workbench.action.terminal.toggleTerminal"
  },
  {
    "key": "cmd+r",
    "command": "renameFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !inputFocus"
  },
  {
    "key": "enter",
    "command": "-renameFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "shift+p shift+p",
    "command": "copyRelativeFilePath",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "shift+alt+cmd+c",
    "command": "-copyRelativeFilePath",
    "when": "!editorFocus"
  },
  {
    "key": "shift+p shift+l",
    "command": "copyFilePath",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+cmd+c",
    "command": "-copyFilePath",
    "when": "!editorFocus"
  },
  {
    "key": "shift+cmd+\\",
    "command": "openInTerminal",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },

  {
    "key": "cmd+a",
    "command": "explorer.newFile",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "shift+cmd+a",
    "command": "explorer.newFolder",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "cmd+\\",
    "command": "-workbench.action.terminal.split",
    "when": "terminalFocus"
  },
  {
    "key": "ctrl+shift+5",
    "command": "-workbench.action.terminal.split",
    "when": "terminalFocus"
  },
  {
    "key": "alt+down",
    "command": "workbench.action.terminal.kill",
    "when": "terminalFocus"
  },
  {
    "key": "shift+cmd+c",
    "command": "editor.action.copyLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+shift+",
    "command": "editor.action.copyLinesUpAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "shift+cmd+2",
    "command": "workbench.action.toggleSidebarVisibility"
  },
  {
    "key": "cmd+b",
    "command": "-workbench.action.toggleSidebarVisibility"
  },
  {
    "key": "shift+cmd+1",
    "command": "workbench.action.toggleActivityBarVisibility"
  },
  {
    "key": "shift+alt+down",
    "command": "-editor.action.copyLinesDownAction",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+cmd+down",
    "command": "workbench.action.splitEditorDown"
  },
  {
    "key": "alt+cmd+left",
    "command": "workbench.action.splitEditorLeft"
  },
  {
    "key": "alt+cmd+right",
    "command": "workbench.action.splitEditorRight"
  },
  {
    "key": "alt+cmd+up",
    "command": "workbench.action.splitEditorUp"
  },
  {
    "key": "f",
    "command": "filesExplorer.findInFolder",
    "when": "explorerResourceIsFolder && explorerViewletVisible && filesExplorerFocus && !inputFocus && resourceScheme == 'file'"
  },
  {
    "key": "shift+alt+f",
    "command": "-filesExplorer.findInFolder",
    "when": "explorerResourceIsFolder && explorerViewletVisible && filesExplorerFocus && !inputFocus && resourceScheme == 'file'"
  },
  {
    "key": "ctrl+f",
    "command": "editor.action.rename",
    "when": "editorHasRenameProvider && editorTextFocus && !editorReadonly"
  },
  {
    "key": "f2",
    "command": "-editor.action.rename",
    "when": "editorHasRenameProvider && editorTextFocus && !editorReadonly"
  },
  {
    "key": "cmd+r",
    "command": "workbench.action.reloadWindow",
    "when": "textInputFocus && !editorReadonly"
  },
  {
    "key": "cmd+r",
    "command": "-workbench.action.reloadWindow",
    "when": "isDevelopment"
  },
  {
    "key": "alt+up",
    "command": "workbench.action.terminal.splitInActiveWorkspace",
    "when": "terminalFocus"
  },
  {
    "key": "alt+left",
    "command": "workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus"
  },
  {
    "key": "alt+cmd+left",
    "command": "-workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus"
  },
  {
    "key": "alt+cmd+up",
    "command": "-workbench.action.terminal.focusPreviousPane",
    "when": "terminalFocus"
  },
  {
    "key": "alt+right",
    "command": "workbench.action.terminal.focusNextPane",
    "when": "terminalFocus"
  },
  {
    "key": "alt+cmd+right",
    "command": "-workbench.action.terminal.focusNextPane",
    "when": "terminalFocus"
  },
  {
    "key": "shift+cmd+x",
    "command": "editor.action.deleteLines",
    "when": "textInputFocus && !editorReadonly"
  },
  {
    "key": "shift+cmd+k",
    "command": "-editor.action.deleteLines",
    "when": "textInputFocus && !editorReadonly"
  },
  {
    "key": "shift+cmd+d",
    "command": "-workbench.view.debug"
  },
  {
    "key": "shift+cmd+r",
    "command": "workbench.files.action.refreshFilesExplorer",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "alt+cmd+=",
    "command": "workbench.action.zoomIn"
  },
  {
    "key": "cmd+=",
    "command": "-workbench.action.zoomIn"
  },
  {
    "key": "alt+cmd+-",
    "command": "workbench.action.zoomOut"
  },
  {
    "key": "cmd+-",
    "command": "-workbench.action.zoomOut"
  },
  {
    "key": "cmd+\\",
    "command": "workbench.action.focusActiveEditorGroup",
    "when": "explorerViewletVisible && filesExplorerFocus && !explorerResourceIsRoot && !explorerResourceReadonly && !inputFocus"
  },
  {
    "key": "shift+cmd+=",
    "command": "-workbench.action.zoomIn"
  },
  {
    "key": "shift+cmd+-",
    "command": "-workbench.action.zoomOut"
  },
  {
    "key": "cmd+k shift+cmd+right",
    "command": "-workbench.action.moveEditorRightInGroup"
  },
  {
    "key": "cmd+=",
    "command": "workbench.action.nextEditor"
  },
  {
    "key": "shift+cmd+]",
    "command": "-workbench.action.nextEditor"
  },
  {
    "key": "shift+cmd+[",
    "command": "workbench.action.moveEditorToLeftGroup"
  },
  {
    "key": "shift+cmd+]",
    "command": "workbench.action.moveEditorToRightGroup"
  },
  {
    "key": "cmd+[",
    "command": "-editor.action.outdentLines",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "cmd+]",
    "command": "-editor.action.indentLines",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "cmd+k shift+cmd+left",
    "command": "-workbench.action.moveEditorLeftInGroup"
  },
  {
    "key": "cmd+-",
    "command": "workbench.action.previousEditor"
  },
  {
    "key": "shift+cmd+[",
    "command": "-workbench.action.previousEditor"
  },
  {
    "key": "alt+cmd+left",
    "command": "-workbench.action.previousEditor"
  },
  {
    "key": "cmd+j",
    "command": "editor.action.joinLines",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "ctrl+j",
    "command": "-editor.action.joinLines",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "cmd+j",
    "command": "-workbench.action.togglePanel"
  },
  {
    "key": "cmd+[",
    "command": "workbench.action.moveEditorLeftInGroup"
  },
  {
    "key": "cmd+]",
    "command": "workbench.action.moveEditorRightInGroup"
  },
  {
    "key": "cmd+\\",
    "command": "revealInExplorer",
    "when": "editorTextFocus && !editorReadonly"
  },
  {
    "key": "shift+cmd+d",
    "command": "bracket-select.select",
    "when": "editorTextFocus"
  },
  {
    "key": "alt+a",
    "command": "-bracket-select.select",
    "when": "editorTextFocus"
  },
  {
    "key": "cmd+.",
    "command": "editor.fold",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "alt+cmd+[",
    "command": "-editor.fold",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+,",
    "command": "editor.unfold",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "alt+cmd+]",
    "command": "-editor.unfold",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+.",
    "command": "editor.toggleFold",
    "when": "editorTextFocus && foldingEnabled"
  },
  {
    "key": "cmd+k cmd+l",
    "command": "-editor.toggleFold",
    "when": "editorTextFocus && foldingEnabled"
  }
]
```
