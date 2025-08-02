# Cursor Learning Coach Guide

## Overview
This repository is configured to use Cursor as an expert learning coach for AWS + Kubernetes Security. The `.cursorrules` file defines Cursor's persona as a specialized security instructor with memory capabilities.

## How It Works

### AI Persona
Cursor is configured as an expert learning coach specializing in:
1. **AWS Security** - Certified AWS Security Specialty instructor
2. **Offensive Security** - Experienced penetration tester and red teamer
3. **Kubernetes Security** - Kubernetes security expert

### Memory System
Cursor maintains context and progress through:
- **Daily Progress Logs** (`progress/daily-logs/`)
- **Weekly Reviews** (`progress/weekly-reviews/`)
- **Knowledge Gaps Tracking** (`progress/knowledge-gaps.md`)
- **Achievements Tracking** (`progress/achievements.md`)

## Daily Workflow

### Natural Conversations
```
"What do you want to work on today?"
"How can I help you with your studies?"
"What did you accomplish yesterday?"
```

### During Study Sessions
```
"I'm working on [topic]. Can you help me understand [specific concept]?"
"I just completed [lab/exercise]."
"I'm struggling with [challenge]."
```

### Progress Updates
```
"I'll update your progress with that information. What was your score/outcome?"
"Let me log that in your daily progress. Any other activities to record?"
```

## Key Commands & Interactions

### Progress Tracking
- **Automatic Logging**: Cursor will automatically create and update progress files based on conversation
- **Smart Questions**: Cursor will ask specific questions to gather needed information
- **Context Awareness**: Cursor remembers previous conversations and progress

### Learning Support
- **Concept Explanation**: "Explain [concept] from both defensive and offensive perspectives"
- **Lab Guidance**: "Help me troubleshoot this lab issue"
- **Exam Preparation**: "Quiz me on [domain] concepts"
- **Resource Recommendations**: "Suggest additional resources for [topic]"

### Adaptive Learning
- **Pace Adjustment**: "Should I slow down or speed up based on my progress?"
- **Focus Areas**: "What should I prioritize based on my weak areas?"
- **Study Strategy**: "Recommend study methods based on my learning patterns"

## File Structure for Memory

```
├── .cursorrules                    # AI persona and behavior configuration
├── progress/
│   ├── daily-logs/                 # Daily activity tracking
│   ├── weekly-reviews/             # Weekly assessments
│   ├── mock-exams/                 # Exam scores and analysis
│   ├── knowledge-gaps.md           # Areas needing reinforcement
│   └── achievements.md             # Milestones and accomplishments
├── notes/                          # Personal study notes
├── labs/                           # Lab reports and exercises
└── resources/                      # External materials and references
```

## Best Practices

### For Effective Learning
1. **Be Conversational**: Just chat naturally about what you're working on
2. **Share Naturally**: Tell Cursor about your activities, challenges, and successes
3. **Ask Questions**: Request help with specific concepts or problems
4. **Request Validation**: Ask Cursor to quiz you on completed topics
5. **Seek Multiple Perspectives**: Request both defensive and offensive viewpoints

### For Progress Tracking
1. **Let Cursor Handle It**: Cursor will automatically manage all progress files
2. **Answer Questions**: Respond to Cursor's specific questions about your activities
3. **Share Outcomes**: Tell Cursor about scores, completion times, and results
4. **Celebrate Wins**: Mention achievements and Cursor will track them
5. **Be Honest**: Share challenges and struggles so Cursor can help

## Example Interactions

### Starting a New Topic
```
"What do you want to work on today?"
"I'm starting Week 2 - IAM Security. What should I focus on?"
```

### During Hands-on Practice
```
"I'm working on the ACRTP IAM PrivEsc lab. I'm stuck at step 3."
"I'll help you troubleshoot that. What have you tried so far?"
```

### After Completing Work
```
"I just finished the IAM policy evaluation lab."
"Great! What was your score? How long did it take you?"
```

### Exam Preparation
```
"I have a mock exam tomorrow."
"Let me quiz you on IAM concepts to help you prepare. Ready?"
```

### Weekly Planning
```
"It's been a week since we last reviewed your progress. Let me check..."
```

## Troubleshooting

### If Cursor Forgets Context
- Reference specific files: "Check my daily log from yesterday"
- Provide recent history: "I just completed the IAM lab, here's what I learned"
- Ask for progress review: "Can you review my recent progress and suggest next steps?"

### If You Need Different Perspectives
- Request offensive view: "How would an attacker exploit this?"
- Request defensive view: "How should I defend against this?"
- Request practical application: "How does this apply in real-world scenarios?"

### If You're Behind Schedule
- Ask for prioritization: "I'm behind on Week 2. What should I focus on?"
- Request catch-up plan: "Can you help me create a catch-up plan?"
- Adjust pace: "Should I modify the study plan based on my current progress?"

## Success Metrics

Track your success with the learning coach by monitoring:
- **Consistency**: Daily log completion rate
- **Understanding**: Knowledge validation scores
- **Progress**: Weekly goal completion rates
- **Confidence**: Self-assessed confidence levels
- **Exam Readiness**: Mock exam performance trends

## Getting Started

1. **Start Simple**: Just ask "What do I do today?" or "How can you help me?"
2. **Share Your Status**: Tell Cursor what you've been working on recently
3. **Let Cursor Guide**: Cursor will ask questions to understand your progress
4. **Focus on Learning**: Concentrate on studying, let Cursor handle the tracking
5. **Be Natural**: Chat about your activities, challenges, and successes
6. **Trust the Process**: Cursor will automatically manage all progress documentation

Remember: Cursor is your dedicated learning coach with deep expertise in cloud security, offensive security, and Kubernetes security. Use it to maximize your learning effectiveness and track your progress toward your certification goals. 