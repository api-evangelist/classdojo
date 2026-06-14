# ClassDojo GraphQL Schema

## Overview

This is a conceptual GraphQL schema for ClassDojo, the classroom communication and student engagement platform connecting teachers, students, and families. ClassDojo does not currently publish a public developer API or GraphQL endpoint. This schema is derived from the platform's documented features — including classroom management, behavior tracking, family messaging, student portfolios, attendance, and the Teacher Toolkit — and represents the data model that would underpin such an API surface.

## Schema Source

- Provider: ClassDojo
- Website: https://www.classdojo.com
- Developer Docs: https://developers.classdojo.com/
- Schema Type: Conceptual
- Coverage: Classroom management, points and behavior, messaging, portfolios, attendance, lessons, badges, events, and administration

## Core Domains

### Classes and Rooms
The `Class` and `ClassDetails` types represent a teacher's classroom with its roster, code, and configuration. `ClassCode` provides the join mechanism for students and parents. `Room` captures the physical or virtual space context.

### Teachers and Staff
`Teacher`, `TeacherDetails`, and `TeacherInfo` model educator accounts, their linked classes, school affiliations, toolkit preferences, and point configurations.

### Students
`Student` and `StudentDetails` hold roster data, point totals, behavior history, attendance records, and portfolio items. `StudentReport` aggregates behavior and skill data over a period.

### Parents and Guardians
`Parent`, `ParentDetails`, `ParentChild`, `Guardian`, and `GuardianDetails` model family accounts, their connected children, and messaging preferences.

### Schools and Directories
`School`, `SchoolDetails`, and `SchoolDirectory` represent institution-level data, administrator accounts, and teacher rosters visible at the school level.

### Messaging
`Message`, `MessageDetails`, `MessageThread`, and `DirectMessage` cover the parent-teacher messaging surface including translation metadata and read receipts. `ClassStory`, `StoryPost`, and `StoryComment` model the class-wide update feed.

### Points and Behavior
`DojoPoint`, `PointDetails`, `PointType`, `Behavior`, `BehaviorDetails`, `BehaviorCategory`, and `PointReport` capture the core behavior feedback loop: assigning positive or constructive feedback points to students using customizable skill labels.

### Portfolios
`Portfolio` and `PortfolioItem` represent student work collections — photos, videos, and notes — shared with families through the app.

### Attendance
`AttendanceRecord` and `Attendance` model daily and period-based attendance check-ins at the class level.

### Lessons and Toolkit
`MiniLesson`, `Lesson`, `Widget`, and `Toolkit` represent the Teacher Toolkit utilities (noise meter, timer, random picker, group maker) and the embedded mini-lesson content library.

### Skills and Moments
`SkillReport`, `SkillDetails`, `Moment`, and `MomentDetails` capture social-emotional learning skill tracking and highlighted memorable classroom moments shared with families.

### Badges and Activities
`Badge`, `BadgeDetails`, and `Activity` represent achievement markers awarded to students and the audit log of platform interactions.

### Events and Groups
`Event`, `EventDetails`, `Group`, and `GroupDetails` model class events, small group configurations within a classroom, and group-level point tracking.

### Authentication and Integration
`APIKey`, `Token`, and `Webhook` represent developer integration primitives for authenticating requests and receiving event notifications.

## Types Summary

| Type | Description |
|------|-------------|
| Class | A teacher's classroom with roster and settings |
| ClassDetails | Extended classroom metadata |
| ClassCode | Join code for students and parents |
| Teacher | Educator account |
| TeacherDetails | Extended teacher profile |
| TeacherInfo | Public-facing teacher information |
| Student | Student account within a class |
| StudentDetails | Extended student profile and totals |
| StudentReport | Aggregated behavior and attendance report |
| Parent | Parent/guardian account |
| ParentDetails | Extended parent profile |
| ParentChild | Parent-to-student connection |
| School | Institution record |
| SchoolDetails | Extended school profile |
| SchoolDirectory | School-level teacher roster |
| Message | Individual message in a thread |
| MessageDetails | Message with translation and metadata |
| MessageThread | Conversation thread between teacher and family |
| DirectMessage | One-to-one direct message |
| ClassStory | Class-wide update feed |
| StoryPost | Post in a class story feed |
| StoryComment | Comment on a story post |
| Portfolio | Student work portfolio |
| PortfolioItem | Individual item in a portfolio |
| Activity | Audit log entry for platform actions |
| DojoPoint | Point awarded to a student |
| PointDetails | Extended point metadata |
| PointType | Custom or default point skill label |
| Behavior | Behavior feedback event |
| BehaviorDetails | Extended behavior metadata |
| BehaviorCategory | Grouping of related behaviors |
| PointReport | Aggregated point summary |
| AttendanceRecord | Single attendance check-in |
| Attendance | Class attendance session |
| MiniLesson | Embedded instructional content unit |
| Lesson | Full lesson record |
| Widget | Teacher Toolkit utility |
| Toolkit | Collection of classroom widgets |
| SkillReport | Social-emotional learning skill summary |
| SkillDetails | Detailed skill definition |
| Moment | Highlighted classroom moment |
| MomentDetails | Extended moment metadata |
| Badge | Achievement badge |
| BadgeDetails | Extended badge metadata |
| Event | Class or school event |
| EventDetails | Extended event metadata |
| Guardian | Legal guardian record |
| GuardianDetails | Extended guardian profile |
| Group | Small group within a class |
| GroupDetails | Extended group metadata |
| Room | Physical or virtual room |
| APIKey | Developer API key credential |
| Token | OAuth or session token |
| Webhook | Event notification subscription |
