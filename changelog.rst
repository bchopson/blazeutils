Changelog
=========

0.6.2 released 2020-07-06
-------------------------

- Add Log Level to Retry Decorator (5ee8d1d_)

.. _5ee8d1d: https://github.com/blazelibs/blazeutils/commit/5ee8d1d


0.6.1 released 2019-11-01
-------------------------

- prepare for release with pyp (e71f222_)
- clean up obsolete decorator usage in favor of wrapt (c1cfb61_)

.. _e71f222: https://github.com/blazelibs/blazeutils/commit/e71f222
.. _c1cfb61: https://github.com/blazelibs/blazeutils/commit/c1cfb61


0.6.0 released 2019-10-30
-------------------------------

- Resolve some python deprecations
- Support python 3.8
- Python 2.7 no longer fully supported

0.5.3 released 2017-12-28
-------------------------------

- Create setup.cfg to build universal wheel
- Create set of functional programming tools

0.5.2 released 2016-11-23
-------------------------------

- Added Python 3.5 compatibility
- Set up CI and coverage

0.5.1 released 2015-05-12
-------------------------------

- Fixed spreadsheets.xlsx_to_reader Python 3.4 compatibility
- Fixed numbers.convert_int exception test for Python 3.4 compatibility
- Fixed case where error handling's _uie_matches masked real exception by creating one

0.5.0 released 2015-03-24
-------------------------------

- Added Python 3.4 compatibility.
- Remove blazeutils.xlrd.  It had been deprecated and the objects moved to .spreadsheets.


0.4.4 released 2014-12-25
-------------------------------

- changed how the version string is determined in __init__.py
- archive old changelog notes

0.4.3 released 2014-12-16
-------------------------------

- add xlsx_to_strio() and WriterX.mwrite()

0.4.2 released 2014-12-08
-------------------------------

- fix wrong dates for 0.4.0 and 0.4.1 releases in changelog
- add roundsecs argument to dates.trim_mils
- updates to spreadsheets module including .xlsx file support

    - xlsx_to_reader(): converts xlsxwriter.Workbook instance to xlrd reader
    - WriterX: like Writer but for xlsxwriter Worksheets, API is slightly different and won't have
      any faculties for style management like Writer does.
    - Reader: gets a .from_xlsx() method
    - http_headers(): utility function to help when sending files as HTTP response

0.4.1 released 2014-05-17
-------------------------------

- fix packaging issue

0.4.0 released 2014-05-17
-------------------------------

- testing.raises() gets support for custom exception validators, docstring updated w/ usage
- decorators.curry() use a different approach so multiple curried functions can be used
- add decorators.hybrid_method() ala SQLAlchemy
- add decorators.memoize() primarily for SQLAlchemy method caching
- BC break: .decorators now uses 'wrapt' so that is a new dependency
