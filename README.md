# Mobile2PC-Remote

┌────────────────────┐
│ Unity Mobile App │
│ (Android) │
│ │
│ UI Buttons │
│ ├─ Volume + │
│ ├─ Volume - │
│ ├─ Mute │
│ └─ Alt + Tab │
└─────────┬──────────┘
│
│ Bluetooth Classic (SPP)
│ Plain Text Commands
│
┌─────────▼──────────┐
│ PC Listener App │
│ (Python) │
│ │
│ Bluetooth COM Port │
│ Command Parser │
│ Action Mapper │
└─────────┬──────────┘
│
│ OS Input Events
│
┌─────────▼──────────┐
│ Operating System │
│ (Keyboard / Media) │
└────────────────────┘
