Changelog
---------

0.3.4 released 2011-06-11
==========================

+ deprecate error_handling.traceback_* functions
+ deprecate datetime module, moved safe_strftime to dates module
+ add decorators.deprecate() decorator
+ add testing.emits_deprecation() decorator (only usable w/ python >= 2.6)
+ add testing.raises() decorator
+ add dates module and ensure_date(), ensure_datetime()

0.3.3 released 2011-05-19
==========================
+ made moneyfmt/decimalfmt handle floats