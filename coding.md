# VScode
## Disable code auto-completion
To disable VSCode’s Copilot suggestions and chat features in the workspace that you are using (i.e., a particular project), you can create a settings.json file inside the ./.vscode directory (relative to the root of the project) with the following content:

```
{
    "github.copilot.enable": { "*" : false },
    "github.copilot.editor.enableAutoCompletions": false,
    "github.copilot.editor.enableCodeActions": false,
    "github.copilot.nextEditSuggestions.enabled": false,
    "github.copilot.renameSuggestions.triggerAutomatically": false,
    "chat.commandCenter.enabled": false,
    "chat.agent.enabled": false
}
```

## 