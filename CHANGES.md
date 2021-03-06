MariaDB4j Release Notes
=======================

v2.2.0 @ 2016-05-05
---

* MAJOR Distribution and project org. split up formerly monolithic MariaDB4j into separate core, exec and binaries artifacts; separately versioned
* @CedricGatay: NEW addArg() method in DBConfigurationBuilder to pass additional flags when spawning a new MariaDB/Mysql process (e.g. like lower_case_table_names, in a mixed OS environment)
* @jahewson: Security related fixed Exception if there are spaces in the data directory path https://github.com/vorburger/MariaDB4j/issues/30
* @timorohwedder: API extended for setting OS dependent library path to optional binary libraries 
* @timorohwedder: Bumped (upgraded) bundled MariaDB Linux version
* Kevin McLaughlin: Synchronize DB install to try to fix some intermittent test failures when running parallel tests in maven that depend on MariaDB4j
* Bumped (upgraded) versions of some 3rd-party Java libraries; thanks https://www.versioneye.com/java/ch.vorburger.mariadb4j:mariadb4j/
* Src: Tabs to Spaces, and enforced by Checkstyle running in Build


v2.1.3 @ 2014-12-27
----

* FIXED Windows package, now tested; it was completely broken in 2.1.1 (but worked in the original 2.1.0)

v2.1.1 @ 2014-12-03
----

* FIXED bad concurrency bug https://github.com/vorburger/MariaDB4j/issues/10
* Upgraded commons-exec v1.2 => v1.3 & Spring Boot v1.1.6 => v1.1.9
* Less annoyingly verbose logging now
* minor code clean-ups etc.

v2.1.0 @ 2014-09-21
------

* Original first public release
  (project existed before without Maven Bintray release; people just built from source)
 
