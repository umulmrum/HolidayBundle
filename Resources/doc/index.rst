
HolidayBundle
=============

Usage
-----

The bundle provides services that simplify usage of the umulmrum/holiday library. All service implementations are
immutable (stateless except for constructor arguments), so they can be used multiple times in a request.
For further documentation please have a look at the umulmrum/holiday library docs.

Filters: `umulmrum_holiday.filter.*` (you might want to define custom filter services to chain filters, though)

Formatters: `umulmrum_holiday.formatter.*` (for formatters that use translations, the Symfony translator is configured automatically)

Translators: `umulmrum_holiday.translator.*` (the Symfony translator is automatically used)

As currently only German holidays are supported, there are only helper services for
Germany yet (although it is easy and welcome both to add own holidays and respective services
and to submit pull requests).

Use `umulmrum_holiday.calculator.holiday_calculator.germany` to calculate holidays

Use `umulmrum_holiday.helper.holiday_helper.germany`

Translations
------------

Translations are provided in the Resources/translations/umulmrum_holiday.*.xliff files. These files are duplicates of
the ones in umulmrum/holiday (it seems that currently there is no sane way to tell Symfony to use translations in another
directory without having to enter the path manually; in the long run it is intended to use the lib files directly).
