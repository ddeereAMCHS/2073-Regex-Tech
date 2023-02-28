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
file1.txt\
***Example Output:***\
192.168.1.1 is a valid IP address\
a.b.c.d is not a valid IP address\
255.255.255.255 is a valid IP address\
312.212.987.432 is not a valid IP address\
0.0.0.0 is a valid IP address\
144.12.12.256 is not a valid IP address\
72.58.19.248 is a valid IP address\
\
http://www.howdy.com is a valid URL\
htp://bad.com is not a valid URL\
https://tamu.edu is a valid URL\
https://ww.what.org is not a valid URL\
https://bye-bye.org is a valid URL\
https://not_gonna_work.com is not a valid URL\
http://www.old3.net is a valid URL\
https://maybe.nope is not a valid URL\
\
valid.txt is a valid filename\
NOT!VALID.jpg is not a valid filenam\
also_valid.pdf is a valid filename\
no.extension is not a valid filenam\
is-valid2.ext is a valid filename\
c#@0$.o is not a valid filenam\
Valid.as.Well.file is a valid filename\
program.c is a valid filename
