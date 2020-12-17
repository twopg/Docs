---
description: View information on 2PG's log events.
---

# Logs

### Log Events

**What are Log Events?**  
Log events allow you to send customizable Discord messages in channels. For example, when a user levels up, we should send the message in the **\#bot-help** channel.

![Level Up Log Event](../.gitbook/assets/image%20%282%29.png)

### Types

These types combine both Discord events and 2PG events.

| Event | Description |
| :--- | :--- |
| Ban | User is banned on Discord |
| Config Update | Bot config is changed |
| Level Up | User reaches a new XP level |
| Member Join | User joins the guild |
| Member Leave | User leaves the guild |
| Message Deleted | User message is deleted |
| Unban | User is unbanned on Discord |
| Warn | User is warned with the `warn` command |

### Event Variables

Event variables are used in the message and provide more context to a message.

| Variable | Description | Example | Events |
| :--- | :--- | :--- | :--- |
| `[GUILD]` | Name of the guild | Test Guild | All |
| `[INSTIGATOR]` | User mention of the punisher |  | WARN |
| `[MEMBER_COUNT]` | Number of members in guild | 420 | All |
| `[MESSAGE]` | Content of a message | Hello Earth | MESSAGE\_DELETED |
| `[MODULE]` | The name of the module that was updated | General | CONFIG\_UPDATE |
| `[NEW_LEVEL]` | The new level of a member | 2 | LEVEL\_UP |
| `[NEW_VALUE]` | The new value of the config | { "prefix": "." } | CONFIG\_UPDATE |
| `[OLD_LEVEL]` | The old level of a member | 1 | LEVEL\_UP |
| `[OLD_VALUE]` | The old value of the config | { "prefix": "/" } | CONFIG\_UPDATE |
| `[REASON]` | Logged reason for punishment | Spamming '🤔' continuously | WARN |
| `[USER]` | User mention |  | All |
| `[XP]` | The current xp of a member | 69425 | LEVEL\_UP |

