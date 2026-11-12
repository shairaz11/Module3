 ┌─────────┐
 │  Start  │
 └────┬────┘
      │
      ▼
┌───────────────────┐
│ Input HoursWorked │
│ Input HourlyRate  │
└─────────┬─────────┘
          │
          ▼
     ┌───────────┐
     │ Hours >40?│
     └─────┬─────┘
      Yes  │  No
           │
           ▼
      ┌───────────────┐
      │ TotalPay =    │
      │ HoursWorked × │
      │ HourlyRate    │
      └──────┬────────┘
             │
             ▼
        ┌─────────┐
        │ Output  │
        │ TotalPay│
        └────┬────┘
             │
             ▼
          ┌─────┐
          │ End │
          └─────┘


YES branch:

┌────────────────────────────┐
│ RegularPay = 40 × Rate     │
│ OvertimeHours = Hours - 40 │
│ OvertimePay =              │
│ OvertimeHours ×            │
│ (Rate × 1.5)              │
│ TotalPay = RegularPay +    │
│ OvertimePay                │
└───────────┬────────────────┘
            │
            ▼
       Output TotalPay
            │
            ▼
           End
