# `estudent-ical`
eStudent iCalendar converter.

This will export the student timetable from the Flinders University Student System into the
iCalendar format, which can be used in Google Calendar or other calendar software.
This may also work with other institutions such as Macquarie University.

## Installation

```console
$ git clone git@github.com:bezborodow/estudent-ical.git
$ cd estudent-ical/
$ sudo apt-get install libdata-ical-perl libdate-calc-perl
$ cpan Date::ICal
```

You may need to reopen your terminal after installing Perl and CPAN.

## Usage

```console
$ ./esical < 2023SI > study2023SI.ics
ENGR1401 Professional Skills
    Lecture-2
        20230227T090000 - 20230227T100000; interval: 1 week; 6 occurances.
        20230424T090000 - 20230424T100000; interval: 1 week; 7 occurances.
    Tutorial
        20230309T150000 - 20230309T160000; interval: 1 week; 5 occurances.
        20230427T150000 - 20230427T160000; interval: 1 week; 7 occurances.
    Workshop
        20230301T160000 - 20230301T180000; interval: 1 week; 6 occurances.
        20230426T160000 - 20230426T180000; interval: 1 week; 7 occurances.
ENGR1711 Engineering Design
    Computer Lab
        20230228T150000 - 20230228T170000; interval: 1 week; 6 occurances.
        20230425T150000 - 20230425T170000; interval: 1 week; 8 occurances.
    Lecture
        20230228T110000 - 20230228T130000; interval: 1 week; 6 occurances.
        20230425T110000 - 20230425T130000; interval: 1 week; 7 occurances.
    Tutorial
        20230307T140000 - 20230307T150000; interval: 1 week; 5 occurances.
        20230502T140000 - 20230502T150000; interval: 1 week; 5 occurances.
ENGR2711 Engineering Mathematics
    Tutorial
        20230309T120000 - 20230309T140000; interval: 1 week; 5 occurances.
        20230427T120000 - 20230427T140000; interval: 1 week; 7 occurances.
    Workshop
        20230309T140000 - 20230309T150000; interval: 1 week; 5 occurances.
        20230427T140000 - 20230427T150000; interval: 1 week; 7 occurances.
ENGR2721 Microprocessors
    Lecture-1
        20230227T120000 - 20230227T130000; interval: 1 week; 6 occurances.
        20230424T120000 - 20230424T130000; interval: 1 week; 7 occurances.
    Lecture-2
        20230301T100000 - 20230301T110000; interval: 1 week; 6 occurances.
        20230426T100000 - 20230426T110000; interval: 1 week; 7 occurances.
    Practical
        20230309T090000 - 20230309T110000; interval: 1 week; 5 occurances.
        20230427T090000 - 20230427T110000; interval: 1 week; 7 occurances.
    Lecture-3
        20230301T150000 - 20230301T160000; interval: 1 week; 6 occurances.
        20230426T150000 - 20230426T160000; interval: 1 week; 7 occurances.

Found 24 events.
Done.
```

## References

 * https://metacpan.org/pod/Data::ICal
 * https://metacpan.org/pod/Data::ICal::Entry
 * https://metacpan.org/pod/Data::ICal::Entry::Event
 * https://metacpan.org/pod/Date::ICal
 * https://icalendar.org/iCalendar-RFC-5545/3-8-5-3-recurrence-rule.html
 * https://www.oreilly.com/library/view/perl-cookbook/1565922433/ch03s06.html
