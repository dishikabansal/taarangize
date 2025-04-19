# FestOrganizer App Structure

## App Architecture
The application will follow MVVM (Model-View-ViewModel) architecture with:
- Activities and Fragments (View)
- ViewModels 
- Repositories
- Firebase Services (Model)

## Package Structure
```
com.your.college.festorganizer
├── data
│   ├── model
│   │   ├── User.kt
│   │   ├── Event.kt
│   │   ├── Task.kt
│   │   ├── Message.kt
│   │   └── Stage.kt
│   ├── repository
│   │   ├── AuthRepository.kt
│   │   ├── EventRepository.kt
│   │   ├── TaskRepository.kt
│   │   └── ChatRepository.kt
│   └── source
│       ├── local
│       └── remote
│           └── FirebaseService.kt
├── ui
│   ├── auth
│   │   ├── LoginFragment.kt
│   │   └── RegisterFragment.kt
│   ├── calendar
│   │   ├── CalendarFragment.kt
│   │   ├── EventDetailsFragment.kt
│   │   └── AddEditEventFragment.kt
│   ├── tasks
│   │   ├── TasksFragment.kt
│   │   ├── TaskDetailsFragment.kt
│   │   └── AssignTaskFragment.kt
│   ├── chat
│   │   ├── ChatFragment.kt
│   │   └── ChatDetailFragment.kt
│   └── main
│       ├── MainActivity.kt
│       └── MainViewModel.kt
└── util
    ├── Extensions.kt
    ├── Constants.kt
    └── NotificationUtil.kt
```

## Feature Components

### 1. Authentication
- Login and Registration screens
- User profiles with roles (Admin, Team Head, Team Member)
- Firebase Authentication integration

### 2. Calendar & Event Management
- Calendar view with three selectable stages
- Event creation, editing, and deletion
- Event details with description, time, location, and assigned teams
- Filter events by stage
- Color coding for different event types

### 3. Task Management
- Create and assign tasks to team members
- Set due dates and priorities
- Mark tasks as in-progress or completed
- Task details view
- Dashboard for team heads to see all assigned tasks

### 4. Chat System
- Group chats for teams
- Direct messaging between users
- Notifications for new messages
- Message read receipts
- Media sharing capabilities

## Database Structure (Firestore)

### Collections

**users**
```
{
  uid: string,
  name: string,
  email: string,
  role: string,
  teamId: string,
  photoUrl: string,
  createdAt: timestamp
}
```

**teams**
```
{
  id: string,
  name: string,
  description: string,
  headId: string,
  members: array<string>
}
```

**events**
```
{
  id: string,
  title: string,
  description: string,
  stageId: string,
  startTime: timestamp,
  endTime: timestamp,
  teamsInvolved: array<string>,
  createdBy: string,
  color: string
}
```

**tasks**
```
{
  id: string,
  title: string,
  description: string,
  assignedTo: string,
  assignedBy: string,
  dueDate: timestamp,
  priority: number,
  status: string,
  teamId: string
}
```

**chats**
```
{
  id: string,
  participants: array<string>,
  isGroupChat: boolean,
  teamId: string,
  lastMessage: string,
  lastMessageTime: timestamp
}
```

**messages**
```
{
  id: string,
  chatId: string,
  senderId: string,
  content: string,
  timestamp: timestamp,
  readBy: array<string>,
  type: string,
  mediaUrl: string
}
```

## Navigation Flow
The app will use a bottom navigation bar with tabs for:
- Calendar
- Tasks
- Chat
- Profile 