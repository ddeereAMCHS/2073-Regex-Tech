# Regex Date/Time

## Due: Tue 2/28 at 11:59 PM

- Create a program called `RegexDateTime.java`
- Prompt the user for a filename containing dates
- Prompt the user for a filename containing times
- Prompt the user for a filename containing datetimes
- Read in all the lines from the dates file into an ArrayList
- Read in all the lines from the times file into another ArrayList
- Read in all the lines from the datetimes file into another ArrayList
- Print whether each date is a valid date or not
  - A date is valid if it follows any of the following formats where months and days can have leading zeroes or not and each number is valid for that field
    - MM-DD-YYYY
    - MM/DD/YYYY
    - MM-DD-YY
    - MM/DD/YY
- Print whether each time is a valid time or not
  - A time is valid if it follows any of the following formats where # is a digit, follows either military time or standard time, and each number is valid for that field (hours can have a leading zero or not)
    - ##:##
    - ##:## AM (not valid if time is in military time)
    - ##:## PM (not valid if time is in military time)
- Print whether each datetime is a valid datetime or not
  - A datetime is valid if it follows the format for date and time
    - A datetime can have the date then the time or the time then the date

***Example Input:***\
date1.txt\
time1.txt\
datetime1.txt\
***Example Output:***\
01/02/03 is a valid date\
13/24/99 is not a valid date\
6-8-1999 is a valid date\
01-02-2003 is a valid date\
5/20/15 is a valid date\
07-43-19 is not a valid date\
07/03/1988 is a valid date\
ab-cd-ef is not a valid date\
11/1/1990 is a valid date\
9-15-05 is a valid date\
12-04-12 is a valid date\
9/2/230 is not a valid date\
\
12:57 is a valid time\
25:32 is not a valid time\
3:43 AM is a valid time\
3:63 is not a valid time\
19:23 is a valid time\
7:43 XM is not a valid time\
19:23 AM is not a valid time\
12:3 is not a valid time\
5:55 is a valid time\
01:23 PM is a valid time\
\
01/02/03 12:57 is a valid datetime\
13/24/99 3:43 AM is not a valid datetime\
25:32 6-8-1999 is not a valid datetime\
01-02-2003 19:23 is a valid datetime\
5/20/15 7:43 XM is not a valid datetime\
07-43-19 3:63 is not a valid datetime\
07/03/1988 5:55 is a valid datetime\
ab-cd-ef 19:23 AM is not a valid datetime\
11/1/1990 5:55 is a valid datetime\
9-15-05 5:55 is a valid datetime\
12-04-12 01:23 PM is a valid datetime\
9/2/230 12:3 is not a valid datetime
