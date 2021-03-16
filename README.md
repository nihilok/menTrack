# menTrack
app for mentor to assign tasks to and track progress of mentees 

### problems to solve:

- save time/energy assigning tasks to mentees
- save time energy reviewing mentees' progress
- reliably track progress / time spent studying
- help second-language speakers of English with tools to aid understanding and learning of terms in resources


### possible means of acheiving goals:

- mentor dashboard with ability to add/track mentees & to create a library of useful links to repeat share with mentees in future and add to pool for other mentors to use
- mentee dashboard with assigned tasks / progress meter
- websocket/gateway server to track time spent using resource.
- tools to easily highlight and save phrases / or google them for more information.
- track said google searches for mentee's own use, and with agreement, mentor's.

### necessary database relationships:

- mentor table
  - mentee set
  - assignments set


- mentee table
  - assignments set
  - mentor ForeignKey


- assignments table
   - mentor
   - mentee
   - completed (bool)


- library table
  - mentor
  - link
  - number of times assigned
  - number of times completed


_possible_ questions/tasks/games

### Security concerns:

- mentor/mentee data breach
- system denial of service (maintaining uptime)

#### Solutions:

- minimal data requirement, e.g PIN no. only
- weak (blind) link to central db e.g HEE database.
- serverside security measures, pentesting



## Minimum Viable Product:

- mobile app to track mentees and send links and messages to mentees
