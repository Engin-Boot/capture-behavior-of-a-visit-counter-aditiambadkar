# Visit-counter for a Director

Scenario: Show patient visits during working days and holidays

  Given foot-fall sensor counter located at patient
entrance door, count is recorded in calendar synced
report generation and patients visit hospital
  When patient enters through patient entrance door and steps on
steps on foot-fall sensor counter
  Then patient count is incremented, recorded and added to working
or holiday patient visit report based on the current day

Scenario: Compute parking slots to reserve for visiting specialists

  Given visiting specialists have fixed timings and days in a week
and it is known they own a car or bike
  When this data is given to car parking system at start of
the day
  Then system automatically reserves parking spots according
to day and time
