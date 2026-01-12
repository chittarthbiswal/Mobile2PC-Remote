# Mobile2PC-Remote
Structured Design 
-Unity - Bluetooth - Listener - OS manipulation
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

#workflow

[Unity Button Click]
↓
Send Command String
↓
Bluetooth Serial Channel
↓
PC Listener Receives Command
↓
Command Mapped to OS Action
↓
System Executes Action
