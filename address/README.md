---
title: Address management README
---
Tools for address management, manipulation, databases etc, so that
you can say "--to mom" instead of some UID or full address when 
addressing a postcard.

The first pass of this is to create some address manipulation tools
in lob.com's API that let you store and address and then subsequently
retrieve it for later use.

What I am realizing from looking at this more is that you need some
kind of bulk import tool, e.g. from a CSV file or database, so that you
can get a bunch of names in fast. The likely path for me personally is
to go in and out of Outlook formatted CSV files since that's a format
also supported by Google Contacts.

Lob has a limit on the size of the address book, based on the plan
that you use. The developer limit is 10000 addresses, which should be
plenty.
