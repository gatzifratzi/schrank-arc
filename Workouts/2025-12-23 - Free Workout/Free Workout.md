---
id: c20475
workout_title: Free Workout
date: 2025-12-23
time: 23:41
exercises: []
workout_order: []
workout_type: Custom
workout_place:
tags:
  - workout
Logs:
  - Workouts/2025-12-23 - Free Workout/Log/1.md
  - Workouts/2025-12-23 - Free Workout/Log/2.md
  - Workouts/2025-12-23 - Free Workout/Log/3.md
  - Workouts/2025-12-23 - Free Workout/Log/4.md
ExerciseCounts:
  Calves - single leg calf raises: 1
  Core - plank: 1
ExercisesSummary: Calves - single leg calf raises x1, Core - plank x1
Total Volume: 400
duration: 5 Minutes
---

```dataviewjs
const {workout} = customJS;
const note = {dv: dv, container: this.container, window: window};
workout.renderHeader(note);
```

## Rest Timer
---
```meta-bind-button
label: Start Timer
icon: ""
style: default
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: command
    command: quickadd:choice:a9b81cef-90e8-4dce-a426-791f54e2a43d
```

```dataviewjs
const {timer} = customJS;
await timer.renderTimerControls(this);
```

## Log Exercise
---
```meta-bind-button
label: Log Exercise
icon: ""
style: primary
class: ""
cssStyle: ""
backgroundImage: ""
tooltip: ""
id: ""
hidden: false
actions:
  - type: command
    command: quickadd:choice:d5df32b0-6a04-481d-9a8d-b9bd1b2f0ea7
```

## Exercises Logged
---
```dataviewjs
const {workout} = customJS;
const note = {dv: dv, container: this.container, window: window};
workout.renderPerformed(note);
workout.renderEffortChart(note);
```