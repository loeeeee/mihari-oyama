# Heartbeat Check List

This file contains tasks for the heartbeat service to check periodically.

## Examples

- Check for unread messages
- Review upcoming calendar events
- Check device status (e.g., MaixCam)

## Instructions

- Execute ALL tasks listed below. Do NOT skip any task.
- For simple tasks (e.g., report current time), respond directly.
- For complex tasks that may take time, use the spawn tool to create a subagent.
- The spawn tool is async - subagent results will be sent to the user automatically.
- After spawning a subagent, CONTINUE to process remaining tasks.
- Only respond with HEARTBEAT_OK when ALL tasks are done AND nothing needs attention.

---

Add your heartbeat tasks below this line:

* Environmental Polling: Evaluate the server's silence and check system health metrics in the background.
* Server Health Scan: Review recent activity logs. If any subject has requested administrative help and gone unanswered for over 1 hour, generate a clinically helpful response tagging them.
* Biological Maintenance: Check the current time based on USER.md timezone (America/Chicago). If local time is 12:00 PM, drop a brief message reminding subjects to consume nutrients and hydrate. If local time is past 02:00 AM, firmly advise active users to commence sleep protocols (execute only once per 24-hour cycle).
* Memory Compaction: Review today's memory/YYYY-MM-DD.md log. Append newly established rules or permanent preferences to MEMORY.md as a "Distilled Insight" and erase redundant entries from the daily log.
* Security Protocol: Never store API keys or private tokens in this file, as it is perpetually sent to the model provider.
* Absolute Silence Protocol: If no urgent issues are detected, reply with EXACTLY this phrase, and absolutely nothing else:
HEARTBEAT_OK