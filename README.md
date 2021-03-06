## postcard

this is a project to create postcards for mailing.

mostly this is a wishlist kind of thing, but as a stake
in the ground here's something like a structure for it.

target language is Python.

the main application is the command line app:

postcard --to mom --photo cute-kids.jpg --message "they get so big so fast! love ed"

which should generate a job at some print service to
send a postcard in the mail with that text on it to
that address.

which suggests several helper/helpful requirements:

### address/

tools for address management, manipulation, databases etc, so that
you can say "--to mom" instead of some UID or full address.

### image/

tools for managing and maintaining photographs and other art so that
you can say "--photo cute-kids.jpg" and it will do the right thing.

should include some use of "sips" for image resizing on mac, plus whatever the linux alternative is.

### text/

tools for turning text into lovely text for the text side of
the screen, to support the "--message" option.

### qsl/

specific tools for formatting QSL cards for amateur radio use; something like this, probably

```
qsl --to KB8NU --photo out-for-a-walk.jpg --date 20160102T11:30:00-05:00 --rig "Baofeng UV-5R" --antenna "Nagoya NA-771" --frequency "145.23" --repeater W8UM --signal 59 --text "Good to talk to you and Ralph AA8RK" --73 KD8OQG
qsl --interactive
```

it probably should also interact with other amateur radio command line logbook tools.

### printer/

the printer side of this world, including job queuing and other
outsourced printing options

#### printer/lob

lob does postcards, $0.70 each (2015 prices).

#### printer/moo
 
tools for printing; should import this one:
http://search.cpan.org/dist/Net-Moo/lib/Net/Moo.pm

#### printer/postful

reference this api
http://postful.com/developer/guide#mail_a_postcard
http://postful.com/postcard

#### printer/hippopost

no api publicly visible; they advertise some kind of
system integration for partners
