# Sample Data for Testing

This document provides sample data that can be used for testing the FestOrganizer app during development.

## User Accounts

```json
[
  {
    "uid": "admin1",
    "name": "Admin User",
    "email": "admin@college.edu",
    "role": "admin",
    "teamId": "",
    "photoUrl": "",
    "createdAt": "2023-10-01T10:00:00Z"
  },
  {
    "uid": "head1",
    "name": "Technical Head",
    "email": "tech.head@college.edu",
    "role": "team_head",
    "teamId": "team1",
    "photoUrl": "",
    "createdAt": "2023-10-01T10:30:00Z"
  },
  {
    "uid": "head2",
    "name": "Cultural Head",
    "email": "cultural.head@college.edu",
    "role": "team_head",
    "teamId": "team2",
    "photoUrl": "",
    "createdAt": "2023-10-01T11:00:00Z"
  },
  {
    "uid": "member1",
    "name": "John Smith",
    "email": "john.smith@college.edu",
    "role": "team_member",
    "teamId": "team1",
    "photoUrl": "",
    "createdAt": "2023-10-01T12:00:00Z"
  },
  {
    "uid": "member2",
    "name": "Emily Johnson",
    "email": "emily.johnson@college.edu",
    "role": "team_member",
    "teamId": "team1",
    "photoUrl": "",
    "createdAt": "2023-10-01T12:30:00Z"
  },
  {
    "uid": "member3",
    "name": "Michael Brown",
    "email": "michael.brown@college.edu",
    "role": "team_member",
    "teamId": "team2",
    "photoUrl": "",
    "createdAt": "2023-10-01T13:00:00Z"
  },
  {
    "uid": "member4",
    "name": "Sarah Davis",
    "email": "sarah.davis@college.edu",
    "role": "team_member",
    "teamId": "team2",
    "photoUrl": "",
    "createdAt": "2023-10-01T13:30:00Z"
  }
]
```

## Teams

```json
[
  {
    "id": "team1",
    "name": "Technical Team",
    "description": "Responsible for all technical aspects of the fest including sound, lighting, and stage management.",
    "headId": "head1",
    "members": ["head1", "member1", "member2"]
  },
  {
    "id": "team2",
    "name": "Cultural Committee",
    "description": "Manages all cultural events, performances, and activities.",
    "headId": "head2",
    "members": ["head2", "member3", "member4"]
  },
  {
    "id": "team3",
    "name": "Management",
    "description": "Handles overall coordination, scheduling, and logistics for the fest.",
    "headId": "admin1",
    "members": ["admin1"]
  }
]
```

## Stages

```json
[
  {
    "id": "stage1",
    "name": "Main Stage",
    "description": "The primary stage for major events and performances",
    "capacity": 500
  },
  {
    "id": "stage2",
    "name": "Secondary Stage",
    "description": "Secondary stage for parallel events",
    "capacity": 250
  },
  {
    "id": "stage3",
    "name": "Workshop Area",
    "description": "Dedicated space for workshops and interactive sessions",
    "capacity": 100
  }
]
```

## Events

```json
[
  {
    "id": "event1",
    "title": "Opening Ceremony",
    "description": "Welcome speech by the college principal followed by cultural performances and fest overview.",
    "stageId": "stage1",
    "startTime": "2023-11-15T09:00:00Z",
    "endTime": "2023-11-15T10:30:00Z",
    "teamsInvolved": ["team2", "team1", "team3"],
    "createdBy": "admin1",
    "color": "#4285F4"
  },
  {
    "id": "event2",
    "title": "Technical Workshop",
    "description": "Hands-on workshop on latest web technologies by industry experts.",
    "stageId": "stage3",
    "startTime": "2023-11-15T11:00:00Z",
    "endTime": "2023-11-15T13:00:00Z",
    "teamsInvolved": ["team1"],
    "createdBy": "head1",
    "color": "#0F9D58"
  },
  {
    "id": "event3",
    "title": "Music Competition",
    "description": "Inter-college music competition with solo and group performances.",
    "stageId": "stage2",
    "startTime": "2023-11-15T14:00:00Z",
    "endTime": "2023-11-15T16:00:00Z",
    "teamsInvolved": ["team2"],
    "createdBy": "head2",
    "color": "#DB4437"
  },
  {
    "id": "event4",
    "title": "Hackathon Kickoff",
    "description": "24-hour coding competition with exciting problem statements and prizes.",
    "stageId": "stage3",
    "startTime": "2023-11-16T09:00:00Z",
    "endTime": "2023-11-16T10:00:00Z",
    "teamsInvolved": ["team1"],
    "createdBy": "head1",
    "color": "#F4B400"
  },
  {
    "id": "event5",
    "title": "Dance Competition",
    "description": "Group dance competition with multiple categories.",
    "stageId": "stage1",
    "startTime": "2023-11-16T11:00:00Z",
    "endTime": "2023-11-16T13:30:00Z",
    "teamsInvolved": ["team2"],
    "createdBy": "head2",
    "color": "#DB4437"
  },
  {
    "id": "event6",
    "title": "Guest Lecture",
    "description": "Industry insights from a renowned tech leader.",
    "stageId": "stage2",
    "startTime": "2023-11-16T14:00:00Z",
    "endTime": "2023-11-16T15:30:00Z",
    "teamsInvolved": ["team1", "team3"],
    "createdBy": "admin1",
    "color": "#4285F4"
  },
  {
    "id": "event7",
    "title": "Closing Ceremony",
    "description": "Prize distribution and vote of thanks.",
    "stageId": "stage1",
    "startTime": "2023-11-17T16:00:00Z",
    "endTime": "2023-11-17T18:00:00Z",
    "teamsInvolved": ["team1", "team2", "team3"],
    "createdBy": "admin1",
    "color": "#4285F4"
  }
]
```

## Tasks

```json
[
  {
    "id": "task1",
    "title": "Prepare Opening Ceremony Script",
    "description": "Write and finalize the script for the opening ceremony including the welcome speech and announcements.",
    "assignedTo": "member3",
    "assignedBy": "head2",
    "dueDate": "2023-11-10T18:00:00Z",
    "priority": 2,
    "status": "pending",
    "teamId": "team2"
  },
  {
    "id": "task2",
    "title": "Design Banners for Main Stage",
    "description": "Create digital designs for the banners to be displayed on the Main Stage during the fest.",
    "assignedTo": "member4",
    "assignedBy": "head2",
    "dueDate": "2023-11-08T18:00:00Z",
    "priority": 1,
    "status": "pending",
    "teamId": "team2"
  },
  {
    "id": "task3",
    "title": "Coordinate with Sound Team",
    "description": "Discuss requirements and setup for all three stages with the sound engineering team.",
    "assignedTo": "member1",
    "assignedBy": "head1",
    "dueDate": "2023-11-12T18:00:00Z",
    "priority": 0,
    "status": "pending",
    "teamId": "team1"
  },
  {
    "id": "task4",
    "title": "Finalize Event Schedule",
    "description": "Review and confirm the final schedule for all events across all three stages.",
    "assignedTo": "member3",
    "assignedBy": "admin1",
    "dueDate": "2023-11-05T18:00:00Z",
    "priority": 2,
    "status": "in_progress",
    "teamId": "team2"
  },
  {
    "id": "task5",
    "title": "Book Main Stage",
    "description": "Reserve the main stage for the fest dates with the college administration.",
    "assignedTo": "head1",
    "assignedBy": "admin1",
    "dueDate": "2023-11-01T18:00:00Z",
    "priority": 2,
    "status": "completed",
    "teamId": "team1"
  },
  {
    "id": "task6",
    "title": "Create Volunteer Schedule",
    "description": "Organize and assign volunteers for various tasks during the fest.",
    "assignedTo": "member2",
    "assignedBy": "head1",
    "dueDate": "2023-11-02T18:00:00Z",
    "priority": 1,
    "status": "completed",
    "teamId": "team1"
  }
]
```

## Chats

```json
[
  {
    "id": "chat1",
    "participants": ["head1", "member1", "member2"],
    "isGroupChat": true,
    "teamId": "team1",
    "lastMessage": "Sound system is ready",
    "lastMessageTime": "2023-11-01T10:45:00Z"
  },
  {
    "id": "chat2",
    "participants": ["head2", "member3", "member4"],
    "isGroupChat": true,
    "teamId": "team2",
    "lastMessage": "We need more volunteers for the dance competition",
    "lastMessageTime": "2023-10-31T14:20:00Z"
  },
  {
    "id": "chat3",
    "participants": ["head1", "head2", "admin1"],
    "isGroupChat": true,
    "teamId": "team3",
    "lastMessage": "Please review the schedule",
    "lastMessageTime": "2023-10-30T09:15:00Z"
  },
  {
    "id": "chat4",
    "participants": ["member1", "member2"],
    "isGroupChat": false,
    "teamId": "",
    "lastMessage": "Let me know when you're free to discuss the sound setup",
    "lastMessageTime": "2023-10-29T16:45:00Z"
  },
  {
    "id": "chat5",
    "participants": ["head1", "member3"],
    "isGroupChat": false,
    "teamId": "",
    "lastMessage": "Thanks for the update!",
    "lastMessageTime": "2023-10-25T11:30:00Z"
  }
]
```

## Messages

```json
[
  {
    "id": "msg1",
    "chatId": "chat1",
    "senderId": "head1",
    "content": "Sound system specs received from the vendor",
    "timestamp": "2023-10-31T10:30:00Z",
    "readBy": ["head1", "member1", "member2"],
    "type": "text",
    "mediaUrl": ""
  },
  {
    "id": "msg2",
    "chatId": "chat1",
    "senderId": "member1",
    "content": "Can someone create a task for setup?",
    "timestamp": "2023-10-31T11:15:00Z",
    "readBy": ["head1", "member1", "member2"],
    "type": "text",
    "mediaUrl": ""
  },
  {
    "id": "msg3",
    "chatId": "chat1",
    "senderId": "member2",
    "content": "I'll handle it",
    "timestamp": "2023-10-31T11:20:00Z",
    "readBy": ["head1", "member1", "member2"],
    "type": "text",
    "mediaUrl": ""
  },
  {
    "id": "msg4",
    "chatId": "chat1",
    "senderId": "head1",
    "content": "Sound system is ready",
    "timestamp": "2023-11-01T10:45:00Z",
    "readBy": ["head1", "member2"],
    "type": "text",
    "mediaUrl": ""
  },
  {
    "id": "msg5",
    "chatId": "chat1",
    "senderId": "member1",
    "content": "Great! I'll inform the organizers",
    "timestamp": "2023-11-01T10:50:00Z",
    "readBy": ["head1"],
    "type": "text",
    "mediaUrl": ""
  }
]
```

## How to Use This Sample Data

1. **Import to Firebase**:
   - Go to your Firebase Console
   - Navigate to Firestore
   - Create collections for each data type
   - Import the data into the respective collections

2. **For Local Testing**:
   - Create helper classes to load this data into your app during development
   - For example:

   ```kotlin
   object SampleDataLoader {
       fun loadEvents(): List<Event> {
           // Parse the JSON sample data
           return listOf(
               Event(
                   id = "event1",
                   title = "Opening Ceremony",
                   description = "Welcome speech by the college principal followed by cultural performances and fest overview.",
                   stageId = "stage1",
                   startTime = Date(1637055600000), // 2023-11-15T09:00:00Z in milliseconds
                   endTime = Date(1637060400000),   // 2023-11-15T10:30:00Z in milliseconds
                   teamsInvolved = listOf("team2", "team1", "team3"),
                   createdBy = "admin1",
                   color = "#4285F4"
               ),
               // Add more events...
           )
       }
       
       // Similar methods for other data types
   }
   ```

3. **Authentication Testing**:
   - Create these accounts in Firebase Authentication
   - Use the email/password authentication method for easy testing

4. **UI Testing**:
   - Use the events and tasks data to populate your UI components
   - Test calendar functionality with the provided event data
   - Verify task filtering and sorting with the diverse task statuses and priorities 