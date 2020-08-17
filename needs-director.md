# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given foot-fall sensor counter located at patient
entrance door, calendar synced report generation records count
and patients visit hospital
  When patient enters through patient entrance door and steps on
steps on foot-fall sensor counter
  Then patient count is incremented, recorded and added to working
or holiday patient visit report based on the current day

Scenario: Compute parking slots to reserve for visiting specialists

  Given visiting specialists have fixed timings and days in a week
and they own a car
  When the car parking system gets visiting specialist data
at start of the day
  Then system automatically reserves parking spots according
to day and time
