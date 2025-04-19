# UI Design Specifications

## Color Palette

```
Primary: #6200EE (Purple)
Primary Variant: #3700B3 (Dark Purple)
Secondary: #03DAC6 (Teal)
Secondary Variant: #018786 (Dark Teal)
Background: #FFFFFF (White)
Surface: #FFFFFF (White)
Error: #B00020 (Red)
On Primary: #FFFFFF (White)
On Secondary: #000000 (Black)
On Background: #000000 (Black)
On Surface: #000000 (Black)
On Error: #FFFFFF (White)
```

## Typography

```
Headline 1: Roboto Light, 96sp
Headline 2: Roboto Light, 60sp
Headline 3: Roboto Regular, 48sp
Headline 4: Roboto Regular, 34sp
Headline 5: Roboto Regular, 24sp
Headline 6: Roboto Medium, 20sp
Subtitle 1: Roboto Regular, 16sp
Subtitle 2: Roboto Medium, 14sp
Body 1: Roboto Regular, 16sp
Body 2: Roboto Regular, 14sp
Button: Roboto Medium, 14sp, ALL CAPS
Caption: Roboto Regular, 12sp
Overline: Roboto Regular, 10sp, ALL CAPS
```

## Screen Mockups

### 1. Login Screen

```
+---------------------------------------+
|                                       |
|                                       |
|             FestOrganizer             |
|                                       |
|  +-------------------------------+    |
|  |           Email               |    |
|  +-------------------------------+    |
|                                       |
|  +-------------------------------+    |
|  |          Password             |    |
|  +-------------------------------+    |
|                                       |
|  +-------------------------------+    |
|  |            LOGIN              |    |
|  +-------------------------------+    |
|                                       |
|         Don't have an account?        |
|            Register here              |
|                                       |
+---------------------------------------+
```

### 2. Main Screen with Calendar

```
+---------------------------------------+
| FestOrganizer           Profile Icon  |
|---------------------------------------|
| [Main] [Secondary] [Workshop]         |
|---------------------------------------|
|        October 2023                   |
|  Mo Tu We Th Fr Sa Su                 |
|   2  3  4  5  6  7  8                 |
|   9 10 11 12 13 14 15                 |
|  16 17 18 19 20 21 22                 |
|  23 24 25 26 27 28 29                 |
|  30 31                                |
|---------------------------------------|
| Events for October 15, 2023           |
|                                       |
| 09:00 - 10:30 | Opening Ceremony      |
| Location: Main Stage                  |
|                                       |
| 11:00 - 13:00 | Technical Workshop    |
| Location: Workshop Area               |
|                                       |
| 14:00 - 16:00 | Music Competition     |
| Location: Secondary Stage             |
|                                       |
|                  [+] Add Event        |
|---------------------------------------|
| [Calendar] [Tasks] [Chat] [Profile]   |
+---------------------------------------+
```

### 3. Event Details Screen

```
+---------------------------------------+
| ← Event Details                       |
|---------------------------------------|
|                                       |
| Opening Ceremony                      |
|                                       |
| Date: October 15, 2023                |
| Time: 09:00 - 10:30                   |
| Location: Main Stage                  |
|                                       |
| Description:                          |
| Welcome speech by the college         |
| principal followed by cultural        |
| performances and fest overview.       |
|                                       |
| Teams Involved:                       |
| • Cultural Committee                  |
| • Technical Team                      |
| • Management                          |
|                                       |
| Created by: Admin                     |
|                                       |
| [Edit]        [Delete]                |
|                                       |
+---------------------------------------+
```

### 4. Tasks Screen

```
+---------------------------------------+
| Tasks                      Filter ⌄   |
|---------------------------------------|
| My Tasks | Assigned by Me             |
|---------------------------------------|
|                                       |
| PENDING (3)                           |
|                                       |
| Prepare Opening Ceremony Script       |
| Due: Oct 10, 2023 | High Priority     |
|                                       |
| Design Banners for Main Stage         |
| Due: Oct 8, 2023 | Medium Priority    |
|                                       |
| Coordinate with Sound Team            |
| Due: Oct 12, 2023 | Low Priority      |
|                                       |
| IN PROGRESS (1)                       |
|                                       |
| Finalize Event Schedule               |
| Due: Oct 5, 2023 | High Priority      |
|                                       |
| COMPLETED (2)                         |
|                                       |
| Book Main Stage                       |
| Completed: Oct 1, 2023                |
|                                       |
| Create Volunteer Schedule             |
| Completed: Oct 2, 2023                |
|                                       |
|                 [+] Add Task          |
|---------------------------------------|
| [Calendar] [Tasks] [Chat] [Profile]   |
+---------------------------------------+
```

### 5. Add/Edit Task Screen

```
+---------------------------------------+
| ← New Task                            |
|---------------------------------------|
|                                       |
| Task Title:                           |
| +-------------------------------+     |
| | Coordinate with Sound Team    |     |
| +-------------------------------+     |
|                                       |
| Description:                          |
| +-------------------------------+     |
| | Discuss requirements and      |     |
| | setup for all three stages    |     |
| | with the sound engineering    |     |
| | team.                         |     |
| +-------------------------------+     |
|                                       |
| Assigned To:                          |
| [       Select Team Member     ⌄ ]    |
|                                       |
| Due Date:                             |
| [ October 12, 2023           📅 ]     |
|                                       |
| Priority:                             |
| O Low    ● Medium    O High           |
|                                       |
| Team:                                 |
| [ Technical Team             ⌄ ]      |
|                                       |
| [ SAVE TASK ]                         |
|                                       |
+---------------------------------------+
```

### 6. Chat List Screen

```
+---------------------------------------+
| Chats                     [+] New     |
|---------------------------------------|
|                                       |
| 🔍 Search chats                       |
|                                       |
| Technical Team                   📱   |
| John: Sound system is ready           |
| 10:45 AM                              |
|                                       |
| Cultural Committee               📱   |
| Sarah: We need more volunteers...     |
| Yesterday                             |
|                                       |
| Management                        📱  |
| You: Please review the schedule       |
| 2d ago                                |
|                                       |
| David Miller                          |
| Let me know when you're free          |
| 3d ago                                |
|                                       |
| Emily Johnson                         |
| Thanks for the update!                |
| 1w ago                                |
|                                       |
|---------------------------------------|
| [Calendar] [Tasks] [Chat] [Profile]   |
+---------------------------------------+
```

### 7. Chat Detail Screen

```
+---------------------------------------+
| ← Technical Team                      |
|---------------------------------------|
|                                       |
|                  Yesterday            |
|                                       |
|           Sound system specs received |
|           from the vendor             |
|                           10:30 AM    |
|                                       |
| Can someone create                    |
| a task for setup?                     |
| 11:15 AM                              |
|                                       |
|           I'll handle it              |
|                           11:20 AM    |
|                                       |
|           Sound system is ready       |
|                           10:45 AM    |
|                                       |
| Great! I'll inform                    |
| the organizers                        |
| 10:50 AM                              |
|                                       |
|---------------------------------------|
| +-----------------------------+  📎   |
| | Type a message...           |  🎤   |
| +-----------------------------+  📤   |
|---------------------------------------|
| [Calendar] [Tasks] [Chat] [Profile]   |
+---------------------------------------+
```

### 8. Profile Screen

```
+---------------------------------------+
| Profile                 [Edit]        |
|---------------------------------------|
|                                       |
|               👤                      |
|            John Doe                   |
|          Technical Head               |
|                                       |
| Email: john.doe@college.edu           |
| Team: Technical Team                  |
|                                       |
| My Responsibilities:                  |
|                                       |
| • Sound system management             |
| • Stage lighting                      |
| • Technical support                   |
|                                       |
| Team Members:                         |
|                                       |
| • Sarah Johnson                       |
| • Mike Brown                          |
| • Emily Davis                         |
|                                       |
| [Add Team Member]                     |
|                                       |
| [Log Out]                             |
|                                       |
|---------------------------------------|
| [Calendar] [Tasks] [Chat] [Profile]   |
+---------------------------------------+
```

## Component Design

### 1. Event Card

```
+---------------------------------------+
| [COLOR BAR] Title of Event            |
| Date & Time                           |
| Location: Stage Name                  |
+---------------------------------------+
```

### 2. Task Card

```
+---------------------------------------+
| Task Title                    [STATUS]|
| Due: Date | Priority                  |
| Assigned by: Name                     |
+---------------------------------------+
```

### 3. Stage Selector

```
+---------------------------------------+
| [ACTIVE] | [INACTIVE] | [INACTIVE]    |
| Stage 1  | Stage 2    | Stage 3       |
+---------------------------------------+
```

### 4. Calendar Day Cell

```
+-------+
|  15   |
| • • • |
+-------+
```

## Icons and Graphics

The app will use Material Design icons for standard functionality:
- Calendar: calendar_today
- Tasks: assignment
- Chat: chat
- Profile: person
- Add: add
- Edit: edit
- Delete: delete
- Back: arrow_back
- More options: more_vert
- Priority high: priority_high
- Priority medium: drag_handle
- Priority low: low_priority
- Search: search
- Filter: filter_list
- Notification: notifications 