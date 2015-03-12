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