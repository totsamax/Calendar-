📘 Repository Description (README.md)
Calendar Grid with Events (Vanilla JS & React)

This repository contains two implementations of a fully interactive calendar grid with time slots, supporting:
15-minute time steps
Resizable events (drag bottom edge to adjust duration)
Automatic event positioning by time
Multi-column layout for overlapping events
Hour and 15-minute grid lines
Day × Time matrix structure
Both versions reproduce the same behavior:

✔️ Vanilla JavaScript version
✔️ React (functional components + hooks) version

The code is written to be easy to read, extend, and learn from.
This project is ideal for studying DOM rendering, absolute positioning, event collision layout algorithms, and Drag-to-Resize UX patterns.

🚀 Features

  🕒 Time Grid
  Day timeline from 08:00 to 20:00
  15-minute slot height defined by SLOT_HEIGHT
  Light 15-min grid + bold hourly lines
  📅 Day Columns
  5-day layout (Mon–Fri)
  Each day contains its own event list
  Layout automatically adjusts to overlapping events
  
  📌 Events
  
  Each event:
  Has a start/end time (HH:MM)
  Automatically computes:
  vertical position (time offset → pixels)
  height (duration → pixels)
  horizontal position when overlapping (columnIndex / columnsCount)
  
  ↕️ Resizing
  
  Drag the bottom handle to resize an event:
  Snaps to 15-minute increments
  Prevents shrinking below 1 slot
  Prevents expanding past the day boundary
  
  🧩 Technologies
  Vanilla Version
  Pure HTML + CSS + JavaScript
  DOM manipulation
  Mouse event tracking
  Custom layout algorithm for event collisions

  React Version
  React 18 (CDN, no build tools required)
  Functional components (Calendar, TimeColumn, DayColumn, EventBlock)
  useState, useRef, useEffect, useMemo
  Same layout logic as the JS version, adapted to React

📁 Folder Structure
  calendar.html       # Vanilla JS implementation
  calendar-react.html # React implementation (single-file component structure)

🎯 Goals of This Project

This repository demonstrates:
How to build an interactive calendar from scratch
How to convert DOM-driven code into a React component architecture
How to implement a manual layout engine (like Google Calendar)
How to write expandable, well-structured UI logic without external libraries

🛠️ Planned Extensions (optional)

Drag & Drop repositioning of events
Weekly/monthly views
Editable event titles
Persistent storage (localStorage / API)
TypeScript version

📄 License

MIT — free for learning, modification and commercial use.
