About
=====

This is a dirty hack that I wrote to automatically rename media files in the 'standard' episode naming format (`Show.Name.SXXEXX.Some.Group.Tags.avi`) to include the actual episode name as provided by [TVRage](http://tvrage.com). Eventually, I'm hoping to abstact this out into a standalone TVRage library, but for now, it does what I want so I'm putting it up here in case anyone finds it useful.

Installing
==========

The only requirements are [nokogiri](http://nokogiri.org/), and read-write access to the files you're wanting to rename. See `tvrage_rename --help` for help.

Bugs
====

* There is a manual workaround in the code for _American Dad!_. The ! character makes SMB shares blow up, so we have to force it to be _American Dad_ instead.
* The option parsing is atrocious
* The code is still a mess
