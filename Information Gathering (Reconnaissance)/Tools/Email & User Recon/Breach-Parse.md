# Breach-Parse
[Breach-Parse (github.com)](https://github.com/hmaverickadams/breach-parse)

A tool that allows you to parse a list of breached credentials for a particular target and output usernames and passwords to text file.  

Requires download of a breached credentials torrent to `/opt/breach-parse`:   
```
magnet:?xt=urn:btih:7ffbcd8cee06aba2ce6561688cf68ce2addca0a3&dn=BreachCompilation&tr=udp%3A%2F%2Ftracker.openbittorrent.com%3A80&tr=udp%3A%2F%2Ftracker.leechers-paradise.org%3A6969&tr=udp%3A%2F%2Ftracker.coppersurfer.tk%3A6969&tr=udp%3A%2F%2Fglotorrents.pw%3A6969&tr=udp%3A%2F%2Ftracker.opentrackr.org%3A1337
```

Examples:  
`./breach-parse.sh @tesla.com tesla.txt` - Breach data in default location  
`./breach-parse.sh @gmail.com gmail.txt "~/Downloads/BreachCompilation/data"` - Breach data stores in Downloads  