# IoT-based-Medicine-Reminder-and-Monitoring-System

```mermaid
flowchart TD
    A[Mobile App 📱] --> B[Set Alarm Time ⏰]
    B --> C[Send SMS via GSM 📡]
    C --> D[Medicine Box 📦 Receives Schedule]
    D --> E[RTC Stores Time ⏳]
    E --> F[Buzzer + LED Trigger 🔔]
    F --> G{Did Patient Take Pill?}
    G -->|Yes| H[Compartment Switch Activated ✅]
    H --> I[Log Event in SD Card 💾]
    I --> J[Send SMS Confirmation to App/Doctor 📲]
    G -->|No| K[Repeat Alarm 🔔 + Missed Dose Alert ⚠️]
    K --> J
