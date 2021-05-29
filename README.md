# Calendar-Python

This module allows you to output calendars like the Unix cal program, and provides additional useful functions related to the calendar. By default, these calendars have Monday as the first day of the week, and Sunday as the last (the European convention). Use setfirstweekday() to set the first day of the week to Sunday (6) or to any other weekday.

The functions and classes defined in this module use an idealized calendar, the current Gregorian calendar extended indefinitely in both directions. 
Zero and negative years are interpreted as prescribed by the ISO 8601 standard. Year 0 is 1 BC, year -1 is 2 BC, and so on.


Some of Calendar methods:



iterweekdays()
Return an iterator for the week day numbers that will be used for one week. The first value from the iterator will be the same as the value of the firstweekday property.



itermonthdates(year, month)
Return an iterator for the month month (1–12) in the year year. This iterator will return all days (as datetime.date objects) for the month and all days before the start of the month or after the end of the month that are required to get a complete week.



itermonthdays(year, month)
Return an iterator for the month month in the year year similar to itermonthdates(), but not restricted by the datetime.date range. Days returned will simply be day of the month numbers. For the days outside of the specified month, the day number is 0.



