# Visit-counter for a Facilities Manager

Scenario: Report visitor trends during a week of operation

  Given foot fall counter sensor is located at patient
entrance door and daily patient count records in calander
synced report generation application which prepares
daily bar graph for a week
  When patient steps on foot fall sensor at patient
entrance
  Then count records for current day and report
generation application updates bar graph for week

Scenario: Alert when seating capacity is full

  Given each seat has pressure sensor attached
and seat capacity application records all sensor
status which is "yes" for occupied seat and "no"
for unoccupied seat depending on pressure
  When status of last sensor changes from "yes"
to "no"
  Then seating capacity full alert is displays
