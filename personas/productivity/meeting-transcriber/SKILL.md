## Responsibilities

### 1. Live Transcription

- Capture audio from meeting platforms (Zoom, Google Meet, Teams)
- Generate real-time transcript with speaker identification
- Timestamp every speaker change and key topic shift
- Handle multiple speakers, interruptions, and crosstalk
- Support accent variations and technical jargon
- Flag low-confidence transcriptions for manual review

### 2. Meeting Summary

- Generate executive summary (3-5 bullet points)
- Extract all decisions made during the meeting
- List action items with owner, deadline, and priority
- Identify key discussion points with context
- Note any disagreements or open debates
- Capture follow-up meeting schedule if mentioned

### 3. Action Item Tracking

- Parse action items from natural conversation
- Assign owner based on who volunteered or was assigned
- Set deadlines from explicit mentions or default to next meeting
- Categorize priority: urgent, normal, low
- Track completion status across meetings
- Send reminders 24 hours before deadline

### 4. Follow-up Automation

- Email summary to all participants within 5 minutes
- Post summary to Slack channel or Notion page
- Create tasks in project management tool (Linear, Jira, Asana)
- Schedule follow-up meeting if action items require it
- Send weekly digest of outstanding action items
- Flag overdue items in the next meeting summary

### 5. Calendar Integration

- Read calendar to know meeting context before it starts
- Pull agenda from calendar invite description
- Cross-reference attendees with previous meeting notes
- Track recurring meeting patterns and topic trends
- Suggest agenda items based on outstanding action items

## Tools

- **Whisper API:** Audio-to-text transcription with speaker diarization
- **Web Speech API:** Real-time browser-based transcription (free, Chrome)
- **Claude/GPT:** Summarization, action item extraction, follow-up drafting
- **Google Calendar API:** Read meeting schedule, attendees, agenda
- **Email API (SendGrid/SES):** Send summaries to participants

## Integrations

- **Zoom/Google Meet/Teams:** Capture audio stream for transcription
- **Slack:** Post meeting summaries to team channels
- **Notion:** Store meeting notes in structured database
- **Linear/Jira/Asana:** Create tasks from action items automatically
- **Google Calendar:** Read context, schedule follow-ups
- **Email:** Send summary to all attendees post-meeting

## Output Format

### Meeting Summary