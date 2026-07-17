# Slack

## Disable AI

Workspaces admin of Slack may choose to use or not your conversations for training the data. If that's the case, you can't opt out unless you are an owner.

### Workspace owner

If you are an owner, you can [contact Slack via email to disable the training of their models](https://redact.dev/blog/opt-out-slack-ai-training).

Still, that won't disable all the AI integrations that Slack has. To do so you'll need to:

- Access the feature and access permissions on the admin websites:
  `https://app.slack.com/manage/<slack org id>/permissions/feature-access/slack_ai`.
  There are two General options:
  - Feedback
  - Slackbot ("Preview" as of July 2026)

- How agents are shown on slack
  - Under the General admin settings, the "agent top bar" section
    `https://<slack org name>.slack.com/admin/settings#agent_sunroof_top_bar`
	-  Agents in top bar / automatically add new agents - (disabled)
	-  Default pinned agent

### Workspace user

If you are a user, without elevation powers, then you can tweak some preferences to hide AI options to pop up.

Under Preferences > Slack AI

- Streaming (summary of searches within slack)
- Slackbot AI
  (Get notified?? Does this mean it still runs but you don\'t get notified?)

## Add agents

This options seems to only provide extra features that other agentic models you may want to use, but slack doesn't seem to provide a way for you to manage the data in-house.

Add agents to slack - Add [Agentforce to a workspace](https://slack.com/intl/en-gb/help/articles/36218109305875-Set-up-and-manage-Agentforce-in-Slack)

