# `estudent-ical`
eStudent iCalendar converter.

This will export the student timetable from the Flinders University Student System into the
iCalendar format, which can be used in Google Calendar or other calendar software.
This may also work with other institutions such as Macquarie University.

## Usage

```console
$ git clone git@github.com:bezborodow/estudent-ical.git
$ cd estudent-ical/
$ sudo apt-get install libdata-ical-perl libdate-calc-perl
$ cpan Date::ICal
$ ./esical > study.ics
CTRL-D
```

## References

 * https://metacpan.org/pod/Data::ICal
 * https://metacpan.org/pod/Data::ICal::Entry
 * https://metacpan.org/pod/Data::ICal::Entry::Event
 * https://metacpan.org/pod/Date::ICal
 * https://icalendar.org/iCalendar-RFC-5545/3-8-5-3-recurrence-rule.html
 * https://www.oreilly.com/library/view/perl-cookbook/1565922433/ch03s06.html
