# Regex Tech

## Due: Mon 3/6 at 11:59 PM

- Create a program called `RegexTech.java`
- Prompt the user for a filename containing IP addresses
- Prompt the user for a filename containing URLs
- Prompt the user for a filename containing filenames
- Read in all the lines from the IP addresses file into an ArrayList
- Read in all the lines from the URLs file into another ArrayList
- Read in all the lines from the filenames file into another ArrayList
- Print whether each IP address is a valid IP address or not
  - An IP address is valid if it follows the format #.#.#.# where # is a number between 0 and 255
- Print whether each URL is a valid URL or not
  - A URL is valid if it follows the format scheme://host
    - scheme is either http or https
    - host is a valid domain name that follows the format subdomain.topdomain with an optional www. at the start
      - topdomain is one of com, org, net, edu, or gov
      - subdomain is 2 to 63 alphanumeric characters or dash
- Print whether each filename is a valid filename or not
  - A filename is valid if it follows the format name.ext
    - name is any alphanumeric character, digit, dot, underscore, or dash
    - ext is one to four letters

***Example Input:***\
ip1.txt\
url1.txt\
file11.txt\
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
