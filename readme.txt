tpc queries for postgres; templates are modified to avoid errors.

Some rules:

* if a subquery is used in FROM clause directly, give it an alias. (starting with alias_a, ...)
* replace 'days' keywords, e.g., (14 days -> interval '14' day)
