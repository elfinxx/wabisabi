## 2.2.1
Changes:
  - Remove the `ignore_conflicts` option via [#53](https://github.com/gphat/wabisabi/pull/53), thanks [SanCoder-Q](https://github.com/SanCoder-Q)!

## 2.2.0
Changes:
  - Bump to Scala 2.12, including various deps

## 2.1.9
Changes:
  - Bump to Scala 2.11.8
  - Release fuckery

## 2.1.8
Changes:
  - Lazily build request object used for debugging to prevent wasted time when debug is disabled via [#40](https://github.com/gphat/wabisabi/pull/40), thanks [SansCoder-Q](https://github.com/SanCoder-Q)!
  - Bump dispatch dependency to 0.11.3 via [#42](https://github.com/gphat/wabisabi/pull/42), thanks [rafa89](https://github.com/rafa89)!

## 2.1.6
Bugfixes
- Fixed some examples via [#38](https://github.com/gphat/wabisabi/pull/38), thanks [karanveerm](https://github.com/karanveerm)!

Features
- Clients can now be instantiated with headers to facilitate authentication via [#39](https://github.com/gphat/wabisabi/pull/39), thanks [gnomff](https://github.com/gnomff)!

## 2.1.5
Changes:
  - Release stuff, moving to maven central.

## 2.1.4
Features:
  - Add a `uriParameters` argument to `mget` to get specific fields from the documents via [source filtering](https://www.elastic.co/guide/en/elasticsearch/reference/1.4/docs-multi-get.html#mget-source-filtering), thanks [SanCoder-Q](https://github.com/SanCoder-Q)

Improvements:
  - Upgrade to Scala 2.11.7
  - Upgrade to Elasticsearch 1.7.0

## 2.1.2
Features:
  - Add `uriParameters` arg to `search` to expose ElasticSearch's [URI Search](http://www.elastic.co/guide/en/elasticsearch/reference/1.4/search-uri-request.html) feature, thanks [mmollaverdi](https://github.com/mmollaverdi)

## 2.1.1
Bugfixes:
  - Fix some incorrect documention, thanks [mmollaverdi](https://github.com/mmollaverdi)

Features:
  - Add `putSettings` method, thanks [mmollaverdi](https://github.com/mmollaverdi)

## 2.1.0
Bugfixes:
  - Fix broken `refresh` method, thanks [mmollaverdi](https://github.com/mmollaverdi)

Improvements:
  - Upgrade to Scala 2.11.6
  - Upgrade to Elasticsearch 1.5.0

## 2.0.19
Features:
  - Add `getSettings` method, thanks [davidbkemp](https://github.com/davidbkemp)

Bugfixes:
  - Fix that `createIndex` wasn't properly setting any `settings` specified, thanks [davidbkemp](https://github.com/davidbkemp)

Improvements:
  - Improve reuse of code in unit tests, thanks [davidbkemp](https://github.com/davidbkemp)

## 2.0.18
Features:
  - Add multi search, thanks [davidbkemp](https://github.com/davidbkemp)

## 2.0.17

Features:
  - Add `ignoreConflicts` parameter to `putMapping`, thanks [sokrahta](https://github.com/sokrahta)

Improvements:
  - Documented the `putMapping` and `getMapping` methods in the README, thanks [sokrahta](https://github.com/sokrahta)
  - Documented the `shutdown()` method in the README for curious users

## 2.0.16

Features:
  - Add methods for [warmers](http://www.elasticsearch.org/guide/en/elasticsearch/reference/current/indices-warmers.html), thanks [jfenc91](https://github.com/jfenc91)

Bugfixes:
  - Extend testing timeouts in case things get slow with the in-VM ES

## 2.0.15

Features:
  - Start keeping a damned CHANGELOG
  - Bump to Scala 2.11.5
  - Include elasticsearch dep in tests to run in-VM ES for integration tests, thanks [mmollaverdi](https://github.com/mmollaverdi)
  - Add travisci
  - Added suggest, thanks [sokrahta](https://github.com/sokrahta)
