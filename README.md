## tnote

A dead simple command line note taking app for you, built while learning [peewee (ORM)](https://github.com/coleifer/peewee)

## Demo

Watch a live demo of it working here

[![asciicast](https://asciinema.org/a/35224.png)](https://asciinema.org/a/35224)

## Features

- Dead simple to use. Even your granny would be able to use it. No seriously!
- Written in uncomplicated python
- Supports full text search for notes
- Adds timestamp for each note which has been added.

## Installation

1) `$ git clone https://github.com/prodicus/tnote`

2) `$ cd tnote && pip install -r requirements.txt`

Fire it up! :volcano:

3) `$ ./journal.py`

## Contributing

This app was created in a timespan of 2 hours while learning to use peewee. So don't be shy to make some PR's here :smile:

**NOTE**

I am using **Sqlite** as the **db** and the **schema** of the database is like this

```sql
$ sqlite3 diary.db 
-- Loading resources from /home/tasdik/.sqliterc

SQLite version 3.8.6 2014-08-15 11:46:33
Enter ".help" for usage hints.
sqlite> .schema
CREATE TABLE "diaryentry" ("id" INTEGER NOT NULL PRIMARY KEY, "content" TEXT NOT NULL, "timestamp" DATETIME NOT NULL);
sqlite> .tables
diaryentry
sqlite> pragma table_info([diaryentry]);
cid         name        type        notnull     dflt_value  pk        
----------  ----------  ----------  ----------  ----------  ----------
0           id          INTEGER     1                       1         
1           content     TEXT        1                       0         
2           timestamp   DATETIME    1                       0         
sqlite>
```

#### To-do
    
- [ ] Add pip support
- [ ] Encrypt the `.db` file using **Sqlcipher**
- [ ] Add better UI using **urwid**
- [ ] Add tags support for notes
- [ ] Add ability to search for notes using timestamp

## Issues

You can report the bugs at the [issue tracker](https://github.com/prodicus/tnote/issues)

**OR**

You can [tweet me](https://twitter.com/tasdikrahman) if you can't get it to work. In fact, you should tweet me anyway.

## License

Built with ♥ by [Tasdik Rahman](http://tasdikrahman.me) under [MIT License](http://prodicus.mit-license.org)

You can find a copy of the License at http://prodicus.mit-license.org/
