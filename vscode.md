# Disable code auto-completion

To disable VSCode’s Copilot suggestions and chat features in the workspace that you are using (i.e., a particular project), you can create a `settings.json` file inside the ./.vscode directory (relative to the root of the project). This can be populated with settings outlined in https://code.visualstudio.com/docs/agents/reference/ai-settings, although the following subset will likely have the most immediate impact:

```
{
    "chat.commandCenter.enabled": false,
    "workbench.settings.showAISearchToggle": false,
    "github.copilot.editor.enableCodeActions": false,
    "github.copilot.renameSuggestions.triggerAutomatically": false,
    "github.copilot.enable": { "*" : false },
    "github.copilot.nextEditSuggestions.fixes": false,
    "chat.agent.enabled": false
}
```
This allows granular control in disabling certain AI features.

To disable all AI functionality globally for your account on the platform, rather than just a local project context, add the following to the general `settings.json` (CTRL+SHIFT+P > "Preferences: Open User Settings (JSON)"):

```
{
    "chat.disableAIFeatures": true,
}
```

[Next Edit Suggestions](https://code.visualstudio.com/docs/editing/ai-powered-suggestions#_next-edit-suggestions), and the use of agents (see `chat.agent.enabled`), are managed at an organizational level, so you might need to contact your systems administrator to alter these.

# Switch LLM model
To set a local or self-hosted model, (requires [Insiders](https://code.visualstudio.com/insiders/) build):
https://code.visualstudio.com/docs/agent-customization/language-models
