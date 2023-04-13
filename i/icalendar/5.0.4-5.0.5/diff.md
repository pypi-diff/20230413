# Comparing `tmp/icalendar-5.0.4.tar.gz` & `tmp/icalendar-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icalendar-5.0.4.tar", last modified: Thu Dec 29 21:55:51 2022, max compression
+gzip compressed data, was "icalendar-5.0.5.tar", last modified: Thu Apr 13 11:56:09 2023, max compression
```

## Comparing `icalendar-5.0.4.tar` & `icalendar-5.0.5.tar`

### file list

```diff
@@ -1,127 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.413532 icalendar-5.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2022-12-29 21:55:40.000000 icalendar-5.0.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2022-12-29 21:55:40.000000 icalendar-5.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-29 21:55:40.000000 icalendar-5.0.4/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-29 21:55:40.000000 icalendar-5.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    27869 2022-12-29 21:55:51.413532 icalendar-5.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2022-12-29 21:55:40.000000 icalendar-5.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.397532 icalendar-5.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      699 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/maintenance.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2022-12-29 21:55:40.000000 icalendar-5.0.4/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-29 21:55:51.413532 icalendar-5.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2022-12-29 21:55:40.000000 icalendar-5.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.393532 icalendar-5.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.397532 icalendar-5.0.4/src/icalendar/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26597 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/caselessdict.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2869 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/parser_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    31729 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/prop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.405532 icalendar-5.0.4/src/icalendar/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/america_new_york.ics
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.405532 icalendar-5.0.4/src/icalendar/tests/calendars/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/big_bad_calendar.ics
--rw-r--r--   0 runner    (1001) docker     (123)      144 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/broken_ical.ics
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/calendar_with_unicode.ics
--rw-r--r--   0 runner    (1001) docker     (123)      563 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/created_calendar_with_unicode_fields.ics
--rw-r--r--   0 runner    (1001) docker     (123)      235 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_104_broken_calendar.ics
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal.ics
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal_2.ics
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_168_expected_output.ics
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_168_input.ics
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_178_component_with_invalid_name_represented.ics
--rw-r--r--   0 runner    (1001) docker     (123)      112 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_178_custom_component_contains_other.ics
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_178_custom_component_inside_other.ics
--rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_237_fail_to_parse_timezone_with_non_ascii_tzid.ics
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_466_convert_tzid_with_slash.ics
--rw-r--r--   0 runner    (1001) docker     (123)      635 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/issue_466_respect_unique_timezone.ics
--rw-r--r--   0 runner    (1001) docker     (123)      948 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/multiple_calendar_components.ics
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/pr_480_summary_with_colon.ics
--rw-r--r--   0 runner    (1001) docker     (123)       40 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/small_bad_calendar.ics
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/calendars/x_location.ics
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.413532 icalendar-5.0.4/src/icalendar/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_escaped_character1.ics
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_escaped_character2.ics
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_escaped_character3.ics
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_escaped_character4.ics
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_escaped_characters.ics
--rw-r--r--   0 runner    (1001) docker     (123)      200 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_recurrence.ics
--rw-r--r--   0 runner    (1001) docker     (123)      456 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_recurrence_exdates_on_different_lines.ics
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_rsvp.ics
--rw-r--r--   0 runner    (1001) docker     (123)      254 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_unicode_fields.ics
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/event_with_unicode_organizer.ics
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_100_transformed_doctests_into_unittests.ics
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_101_icalendar_chokes_on_umlauts_in_organizer.ics
--rw-r--r--   0 runner    (1001) docker     (123)      164 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_104_mark_events_broken.ics
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_112_missing_tzinfo_on_exdate.ics
--rw-r--r--   0 runner    (1001) docker     (123)      170 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_156_RDATE_with_PERIOD.ics
--rw-r--r--   0 runner    (1001) docker     (123)      198 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_156_RDATE_with_PERIOD_list.ics
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_157_removes_trailing_semicolon.ics
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_184_broken_representation_of_period.ics
--rw-r--r--   0 runner    (1001) docker     (123)      193 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_464_invalid_rdate.ics
--rw-r--r--   0 runner    (1001) docker     (123)      739 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_53_description_parsed_properly.ics
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_64_event_with_ascii_summary.ics
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_64_event_with_non_ascii_summary.ics
--rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_70_rrule_causes_attribute_error.ics
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/events/issue_82_expected_output.ics
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.413532 icalendar-5.0.4/src/icalendar/tests/hypothesis/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/hypothesis/test_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/pacific_fiji.ics
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_cli_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_components_break_on_bad_ics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_fixed_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_icalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_issue_168_parsing_invalid_calendars_no_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_issue_318_skip_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_issue_500_vboolean_for_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_period.py
--rw-r--r--   0 runner    (1001) docker     (123)     5719 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_property_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_recurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_timezoned.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_unit_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_unit_caselessdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_unit_parser_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_unit_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_unit_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/test_with_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/time.ics
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezone_rdate.ics
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezone_same_start.ics
--rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezone_same_start_and_offset.ics
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezoned.ics
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.413532 icalendar-5.0.4/src/icalendar/tests/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezones/issue_237_brazilia_standard.ics
--rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezones/issue_53_tzid_parsed_properly.ics
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tests/timezones/issue_55_parse_error_on_utc_offset_with_seconds.ics
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/timezone_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2022-12-29 21:55:40.000000 icalendar-5.0.4/src/icalendar/windows_to_olson.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 21:55:51.397532 icalendar-5.0.4/src/icalendar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27869 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-29 21:55:51.000000 icalendar-5.0.4/src/icalendar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2022-12-29 21:55:40.000000 icalendar-5.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.254521 icalendar-5.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-04-13 11:55:54.000000 icalendar-5.0.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-13 11:55:54.000000 icalendar-5.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 11:55:54.000000 icalendar-5.0.5/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 11:55:54.000000 icalendar-5.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-04-13 11:56:09.254521 icalendar-5.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-04-13 11:55:54.000000 icalendar-5.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.234521 icalendar-5.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/maintenance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-04-13 11:55:54.000000 icalendar-5.0.5/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-13 11:56:09.258521 icalendar-5.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-13 11:55:54.000000 icalendar-5.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.230521 icalendar-5.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.238521 icalendar-5.0.5/src/icalendar/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26597 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/caselessdict.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2869 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13039 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/parser_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/prop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.246521 icalendar-5.0.5/src/icalendar/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/america_new_york.ics
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.250521 icalendar-5.0.5/src/icalendar/tests/calendars/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/big_bad_calendar.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/broken_ical.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/calendar_with_unicode.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/created_calendar_with_unicode_fields.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_104_broken_calendar.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal_2.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_168_expected_output.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_168_input.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_178_component_with_invalid_name_represented.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_178_custom_component_contains_other.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_178_custom_component_inside_other.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_237_fail_to_parse_timezone_with_non_ascii_tzid.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_348_exception_parsing_value.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_466_convert_tzid_with_slash.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/issue_466_respect_unique_timezone.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/multiple_calendar_components.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/pr_480_summary_with_colon.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/small_bad_calendar.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/calendars/x_location.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.254521 icalendar-5.0.5/src/icalendar/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_escaped_character1.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_escaped_character2.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_escaped_character3.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_escaped_character4.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_escaped_characters.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_recurrence.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_recurrence_exdates_on_different_lines.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_rsvp.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_unicode_fields.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/event_with_unicode_organizer.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_100_transformed_doctests_into_unittests.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_101_icalendar_chokes_on_umlauts_in_organizer.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_104_mark_events_broken.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_112_missing_tzinfo_on_exdate.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_156_RDATE_with_PERIOD.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_156_RDATE_with_PERIOD_list.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_157_removes_trailing_semicolon.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_184_broken_representation_of_period.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_464_invalid_rdate.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_53_description_parsed_properly.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_64_event_with_ascii_summary.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_64_event_with_non_ascii_summary.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_70_rrule_causes_attribute_error.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/events/issue_82_expected_output.ics
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.254521 icalendar-5.0.5/src/icalendar/tests/hypothesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/hypothesis/test_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/pacific_fiji.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_cli_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_components_break_on_bad_ics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_fixed_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_icalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_issue_168_parsing_invalid_calendars_no_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_issue_318_skip_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_issue_348_exception_parsing_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_issue_500_vboolean_for_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_property_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_recurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_timezoned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_unit_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_unit_caselessdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_unit_parser_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21799 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_unit_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_unit_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/test_with_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/time.ics
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezone_rdate.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezone_same_start.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezone_same_start_and_offset.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezoned.ics
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.254521 icalendar-5.0.5/src/icalendar/tests/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezones/issue_237_brazilia_standard.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezones/issue_53_tzid_parsed_properly.ics
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tests/timezones/issue_55_parse_error_on_utc_offset_with_seconds.ics
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/timezone_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-13 11:55:54.000000 icalendar-5.0.5/src/icalendar/windows_to_olson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 11:56:09.238521 icalendar-5.0.5/src/icalendar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-13 11:56:08.000000 icalendar-5.0.5/src/icalendar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-13 11:55:54.000000 icalendar-5.0.5/tox.ini
```

### Comparing `icalendar-5.0.4/CHANGES.rst` & `icalendar-5.0.5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog
 =========
 
+5.0.5 (2023-04-13)
+------------------
+
+Minor changes:
+
+- Added support for BYWEEKDAY in vRecur ref: #268 
+
+Bug fixes:
+
+- Fix problem with ORGANIZER in FREE/BUSY #348
+
 5.0.4 (2022-12-29)
 ------------------
 
 Minor changes:
 
 - Improved documentation
   Ref: #503, #504
```

### Comparing `icalendar-5.0.4/CONTRIBUTING.rst` & `icalendar-5.0.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/LICENSE.rst` & `icalendar-5.0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/PKG-INFO` & `icalendar-5.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalendar
-Version: 5.0.4
+Version: 5.0.5
 Summary: iCalendar parser/generator
 Home-page: https://github.com/collective/icalendar
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: calendar calendaring ical icalendar event todo journal recurring
 Platform: UNKNOWN
@@ -46,19 +46,19 @@
    :target: https://pypi.org/project/icalendar/
    :alt: Python Package Version on PyPI
 
 .. image:: https://img.shields.io/pypi/dm/icalendar.svg
    :target: https://pypi.org/project/icalendar/#files
    :alt: Downloads from PyPI
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/master?label=master&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=master&label=master&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3Amaster
     :alt: GitHub Actions build status for master
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/4.x?label=4.x&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=4.x&label=4.x&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3A4.x++
     :alt: GitHub Actions build status for 4.x
 
 .. image:: https://readthedocs.org/projects/icalendar/badge/?version=latest
     :target: https://icalendar.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
@@ -123,14 +123,25 @@
 contribute changes, the `Installation Section
 <https://icalendar.readthedocs.io/en/latest/install.html>`_
 should help you further.
 
 Changelog
 =========
 
+5.0.5 (2023-04-13)
+------------------
+
+Minor changes:
+
+- Added support for BYWEEKDAY in vRecur ref: #268 
+
+Bug fixes:
+
+- Fix problem with ORGANIZER in FREE/BUSY #348
+
 5.0.4 (2022-12-29)
 ------------------
 
 Minor changes:
 
 - Improved documentation
   Ref: #503, #504
```

### Comparing `icalendar-5.0.4/README.rst` & `icalendar-5.0.5/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -20,19 +20,19 @@
    :target: https://pypi.org/project/icalendar/
    :alt: Python Package Version on PyPI
 
 .. image:: https://img.shields.io/pypi/dm/icalendar.svg
    :target: https://pypi.org/project/icalendar/#files
    :alt: Downloads from PyPI
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/master?label=master&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=master&label=master&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3Amaster
     :alt: GitHub Actions build status for master
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/4.x?label=4.x&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=4.x&label=4.x&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3A4.x++
     :alt: GitHub Actions build status for 4.x
 
 .. image:: https://readthedocs.org/projects/icalendar/badge/?version=latest
     :target: https://icalendar.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
```

### Comparing `icalendar-5.0.4/docs/Makefile` & `icalendar-5.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/docs/about.rst` & `icalendar-5.0.5/docs/about.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/docs/cli.rst` & `icalendar-5.0.5/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/docs/conf.py` & `icalendar-5.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/docs/credits.rst` & `icalendar-5.0.5/docs/credits.rst`

 * *Files 5% similar despite different names*

```diff
@@ -62,11 +62,12 @@
 - Maurits van Rees <maurits@vanrees.org>
 - jacadzaca <vitouejj@gmail.com>
 - Mauro Amico <mauro.amico@gmail.com>
 - Alexander Pitkin <peleccom@gmail.com>
 - Michał Górny <mgorny@gentoo.org>
 - Pronoy <lukex9442@gmail.com>
 - Abe Hanoka <abe@habet.dev>
+- `Natasha Mattson <https://github.com/natashamm`_
 
 Find out who contributed::
 
     $ git shortlog -s -e
```

### Comparing `icalendar-5.0.4/docs/install.rst` & `icalendar-5.0.5/docs/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 .. code-block:: python
 
     Python 3.9.5 (default, Nov 23 2021, 15:27:38)
     Type "help", "copyright", "credits" or "license" for more information.
     >>> import icalendar
     >>> icalendar.__version__
-    '5.0.4'
+    '5.0.5'
 
 Building the documentation locally
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To build the documentation follow these steps:
 
 .. code-block:: bash
```

### Comparing `icalendar-5.0.4/docs/maintenance.rst` & `icalendar-5.0.5/docs/maintenance.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/docs/usage.rst` & `icalendar-5.0.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/setup.py` & `icalendar-5.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/__init__.py` & `icalendar-5.0.5/src/icalendar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '5.0.4'
+__version__ = '5.0.5'
 
 from icalendar.cal import (
     Calendar,
     Event,
     Todo,
     Journal,
     Timezone,
```

### Comparing `icalendar-5.0.4/src/icalendar/cal.py` & `icalendar-5.0.5/src/icalendar/cal.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/caselessdict.py` & `icalendar-5.0.5/src/icalendar/caselessdict.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/cli.py` & `icalendar-5.0.5/src/icalendar/cli.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/parser.py` & `icalendar-5.0.5/src/icalendar/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,16 @@
                         value_split = i
                 if ch == '"':
                     in_quotes = not in_quotes
             name = unescape_string(st[:name_split])
             if not name:
                 raise ValueError('Key name is required')
             validate_token(name)
+            if not value_split:
+                value_split = i + 1
             if not name_split or name_split + 1 == value_split:
                 raise ValueError('Invalid content line')
             params = Parameters.from_ical(st[name_split + 1: value_split],
                                           strict=self.strict)
             params = Parameters(
                 (unescape_string(key), unescape_list_or_string(value))
                 for key, value in iter(params.items())
```

### Comparing `icalendar-5.0.4/src/icalendar/parser_tools.py` & `icalendar-5.0.5/src/icalendar/parser_tools.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/prop.py` & `icalendar-5.0.5/src/icalendar/prop.py`

 * *Files 1% similar despite different names*

```diff
@@ -639,15 +639,15 @@
 
     frequencies = ["SECONDLY", "MINUTELY", "HOURLY", "DAILY", "WEEKLY",
                    "MONTHLY", "YEARLY"]
 
     # Mac iCal ignores RRULEs where FREQ is not the first rule part.
     # Sorts parts according to the order listed in RFC 5545, section 3.3.10.
     canonical_order = ("FREQ", "UNTIL", "COUNT", "INTERVAL",
-                       "BYSECOND", "BYMINUTE", "BYHOUR", "BYDAY",
+                       "BYSECOND", "BYMINUTE", "BYHOUR", "BYDAY", "BYWEEKDAY",
                        "BYMONTHDAY", "BYYEARDAY", "BYWEEKNO", "BYMONTH",
                        "BYSETPOS", "WKST")
 
     types = CaselessDict({
         'COUNT': vInt,
         'INTERVAL': vInt,
         'BYSECOND': vInt,
@@ -658,14 +658,15 @@
         'BYYEARDAY': vInt,
         'BYMONTH': vInt,
         'UNTIL': vDDDTypes,
         'BYSETPOS': vInt,
         'WKST': vWeekday,
         'BYDAY': vWeekday,
         'FREQ': vFrequency,
+        'BYWEEKDAY': vWeekday,
     })
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.params = Parameters()
 
     def to_ical(self):
```

### Comparing `icalendar-5.0.4/src/icalendar/tests/america_new_york.ics` & `icalendar-5.0.5/src/icalendar/tests/america_new_york.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/created_calendar_with_unicode_fields.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/created_calendar_with_unicode_fields.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal_2.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal_2.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/issue_237_fail_to_parse_timezone_with_non_ascii_tzid.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/issue_237_fail_to_parse_timezone_with_non_ascii_tzid.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/issue_466_respect_unique_timezone.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/issue_466_respect_unique_timezone.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/multiple_calendar_components.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/multiple_calendar_components.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/calendars/x_location.ics` & `icalendar-5.0.5/src/icalendar/tests/calendars/x_location.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/conftest.py` & `icalendar-5.0.5/src/icalendar/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/events/issue_112_missing_tzinfo_on_exdate.ics` & `icalendar-5.0.5/src/icalendar/tests/events/issue_112_missing_tzinfo_on_exdate.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/events/issue_53_description_parsed_properly.ics` & `icalendar-5.0.5/src/icalendar/tests/events/issue_53_description_parsed_properly.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/hypothesis/test_fuzzing.py` & `icalendar-5.0.5/src/icalendar/tests/hypothesis/test_fuzzing.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/pacific_fiji.ics` & `icalendar-5.0.5/src/icalendar/tests/pacific_fiji.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_cli_tool.py` & `icalendar-5.0.5/src/icalendar/tests/test_cli_tool.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_components_break_on_bad_ics.py` & `icalendar-5.0.5/src/icalendar/tests/test_components_break_on_bad_ics.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_encoding.py` & `icalendar-5.0.5/src/icalendar/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_examples.py` & `icalendar-5.0.5/src/icalendar/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_fixed_issues.py` & `icalendar-5.0.5/src/icalendar/tests/test_fixed_issues.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_icalendar.py` & `icalendar-5.0.5/src/icalendar/tests/test_icalendar.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_issue_168_parsing_invalid_calendars_no_warning.py` & `icalendar-5.0.5/src/icalendar/tests/test_issue_168_parsing_invalid_calendars_no_warning.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_issue_318_skip_default_parameters.py` & `icalendar-5.0.5/src/icalendar/tests/test_issue_318_skip_default_parameters.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_multiple.py` & `icalendar-5.0.5/src/icalendar/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_parsing.py` & `icalendar-5.0.5/src/icalendar/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_period.py` & `icalendar-5.0.5/src/icalendar/tests/test_period.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_property_params.py` & `icalendar-5.0.5/src/icalendar/tests/test_property_params.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_recurrence.py` & `icalendar-5.0.5/src/icalendar/tests/test_recurrence.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_time.py` & `icalendar-5.0.5/src/icalendar/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_timezoned.py` & `icalendar-5.0.5/src/icalendar/tests/test_timezoned.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_unit_cal.py` & `icalendar-5.0.5/src/icalendar/tests/test_unit_cal.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_unit_caselessdict.py` & `icalendar-5.0.5/src/icalendar/tests/test_unit_caselessdict.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_unit_parser_tools.py` & `icalendar-5.0.5/src/icalendar/tests/test_unit_parser_tools.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_unit_prop.py` & `icalendar-5.0.5/src/icalendar/tests/test_unit_prop.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,26 @@
 
         self.assertEqual(
             vRecur(r).to_ical(),
             b'FREQ=YEARLY;INTERVAL=2;BYMINUTE=30;BYHOUR=8,9;BYDAY=-SU;'
             b'BYMONTH=1'
         )
 
+        r = vRecur.from_ical('FREQ=WEEKLY;INTERVAL=1;BYWEEKDAY=TH')
+        
+        self.assertEqual(
+            r,
+            {'FREQ': ['WEEKLY'], 'INTERVAL': [1], 'BYWEEKDAY': ['TH']}
+        )
+
+        self.assertEqual(
+            vRecur(r).to_ical(),
+            b'FREQ=WEEKLY;INTERVAL=1;BYWEEKDAY=TH'
+        )
+
         # Some examples from the spec
         r = vRecur.from_ical('FREQ=MONTHLY;BYDAY=MO,TU,WE,TH,FR;BYSETPOS=-1')
         self.assertEqual(vRecur(r).to_ical(),
                          b'FREQ=MONTHLY;BYDAY=MO,TU,WE,TH,FR;BYSETPOS=-1')
 
         p = 'FREQ=YEARLY;INTERVAL=2;BYMONTH=1;BYDAY=SU;BYHOUR=8,9;BYMINUTE=30'
         r = vRecur.from_ical(p)
```

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_unit_tools.py` & `icalendar-5.0.5/src/icalendar/tests/test_unit_tools.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/test_with_doctest.py` & `icalendar-5.0.5/src/icalendar/tests/test_with_doctest.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/timezone_rdate.ics` & `icalendar-5.0.5/src/icalendar/tests/timezone_rdate.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/timezone_same_start.ics` & `icalendar-5.0.5/src/icalendar/tests/timezone_same_start.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tests/timezoned.ics` & `icalendar-5.0.5/src/icalendar/tests/timezoned.ics`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/tools.py` & `icalendar-5.0.5/src/icalendar/tools.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar/windows_to_olson.py` & `icalendar-5.0.5/src/icalendar/windows_to_olson.py`

 * *Files identical despite different names*

### Comparing `icalendar-5.0.4/src/icalendar.egg-info/PKG-INFO` & `icalendar-5.0.5/src/icalendar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalendar
-Version: 5.0.4
+Version: 5.0.5
 Summary: iCalendar parser/generator
 Home-page: https://github.com/collective/icalendar
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: calendar calendaring ical icalendar event todo journal recurring
 Platform: UNKNOWN
@@ -46,19 +46,19 @@
    :target: https://pypi.org/project/icalendar/
    :alt: Python Package Version on PyPI
 
 .. image:: https://img.shields.io/pypi/dm/icalendar.svg
    :target: https://pypi.org/project/icalendar/#files
    :alt: Downloads from PyPI
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/master?label=master&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=master&label=master&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3Amaster
     :alt: GitHub Actions build status for master
 
-.. image:: https://img.shields.io/github/workflow/status/collective/icalendar/tests/4.x?label=4.x&logo=github
+.. image:: https://img.shields.io/github/actions/workflow/status/collective/icalendar/tests.yml?branch=4.x&label=4.x&logo=github
     :target: https://github.com/collective/icalendar/actions/workflows/tests.yml?query=branch%3A4.x++
     :alt: GitHub Actions build status for 4.x
 
 .. image:: https://readthedocs.org/projects/icalendar/badge/?version=latest
     :target: https://icalendar.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
@@ -123,14 +123,25 @@
 contribute changes, the `Installation Section
 <https://icalendar.readthedocs.io/en/latest/install.html>`_
 should help you further.
 
 Changelog
 =========
 
+5.0.5 (2023-04-13)
+------------------
+
+Minor changes:
+
+- Added support for BYWEEKDAY in vRecur ref: #268 
+
+Bug fixes:
+
+- Fix problem with ORGANIZER in FREE/BUSY #348
+
 5.0.4 (2022-12-29)
 ------------------
 
 Minor changes:
 
 - Improved documentation
   Ref: #503, #504
```

### Comparing `icalendar-5.0.4/src/icalendar.egg-info/SOURCES.txt` & `icalendar-5.0.5/src/icalendar.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 src/icalendar/tests/test_components_break_on_bad_ics.py
 src/icalendar/tests/test_encoding.py
 src/icalendar/tests/test_examples.py
 src/icalendar/tests/test_fixed_issues.py
 src/icalendar/tests/test_icalendar.py
 src/icalendar/tests/test_issue_168_parsing_invalid_calendars_no_warning.py
 src/icalendar/tests/test_issue_318_skip_default_parameters.py
+src/icalendar/tests/test_issue_348_exception_parsing_value.py
 src/icalendar/tests/test_issue_500_vboolean_for_parameter.py
 src/icalendar/tests/test_multiple.py
 src/icalendar/tests/test_parsing.py
 src/icalendar/tests/test_period.py
 src/icalendar/tests/test_property_params.py
 src/icalendar/tests/test_recurrence.py
 src/icalendar/tests/test_time.py
@@ -76,14 +77,15 @@
 src/icalendar/tests/calendars/issue_156_RDATE_with_PERIOD_TZID_khal_2.ics
 src/icalendar/tests/calendars/issue_168_expected_output.ics
 src/icalendar/tests/calendars/issue_168_input.ics
 src/icalendar/tests/calendars/issue_178_component_with_invalid_name_represented.ics
 src/icalendar/tests/calendars/issue_178_custom_component_contains_other.ics
 src/icalendar/tests/calendars/issue_178_custom_component_inside_other.ics
 src/icalendar/tests/calendars/issue_237_fail_to_parse_timezone_with_non_ascii_tzid.ics
+src/icalendar/tests/calendars/issue_348_exception_parsing_value.ics
 src/icalendar/tests/calendars/issue_466_convert_tzid_with_slash.ics
 src/icalendar/tests/calendars/issue_466_respect_unique_timezone.ics
 src/icalendar/tests/calendars/multiple_calendar_components.ics
 src/icalendar/tests/calendars/pr_480_summary_with_colon.ics
 src/icalendar/tests/calendars/small_bad_calendar.ics
 src/icalendar/tests/calendars/x_location.ics
 src/icalendar/tests/events/event_with_escaped_character1.ics
```

### Comparing `icalendar-5.0.4/tox.ini` & `icalendar-5.0.5/tox.ini`

 * *Files identical despite different names*

