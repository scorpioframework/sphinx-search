Scorpio SphinxSearch Library Change Log
=======================================

2017-09-02
----------

 * updated to PSR4
 * updated tests to PHPUnit only
 * updated dependencies
 * updated docs

2015-09-27 0.2.1
----------------

Added a pseudo query builder type thingy for building query strings in code with
built-in escaping and parenthesis handling.

Made some minor refactorings in SearchIndex for better code re-use.

Added additional helper methods including iterators.

2015-09-26 0.2.0
----------------

Change "filters" in SearchIndex to "attributes". Made all properties parameters in
constructor so SearchIndex does not need to be overridden to set these.

Refactored SearchIndex to use an interface.

2015-09-25 0.1.0
----------------

Remove call to deprecated method setMatchMode. Now uses setRankingMode. Removed all
previous constants and references to MatchMode.

Change SearchManager to use ServerSettings and each query creates a new SphinxClient
instance removing the issues with bound queries not being removable and SphinxClient
not being cloneable.

2015-09-25
----------

Initial commit.
