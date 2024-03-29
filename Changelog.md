# Changelog

## v0.10.2 (08/22/2023)

- Support publishing amd64 and s390x container images

## v0.10.1 (05/11/2023)

- Include tag pushes in docker builds

## v0.10.0 (05/11/2023)

- Multiple documentation updates
- Updated docker-compose syntax
- Upgrade tests to use python3
- Upgrade node base for Docker image
- Automatic container publishing via GHA

## v0.9.0 (08/27/2020)

- Add support for graphite tagged metrics
- Fix dashboard to 0 last_exception time on startup
- Multiple documentation updates
- Correct some out-dated integration examples
- Update container image to use recent node version

## v0.8.6 (02/19/2020)

- Add an optional max TTL setting for gauges
- add filter option for metrics

## v0.8.5 (07/23/2019)

- Update lodash (sub dependency) for security fix
- Add the StatsD history to the docs
- Add third party server interfaces to docs
- Migrate docs from github wiki, and standardise markdown notation
- Minor formatting proposals
- Add docker image info to readme

## v0.8.4 (07/11/2019)

- update modern-syslog to 1.2.0 for node 12 compatibility
- update package.json version to 0.8.3

## v0.8.3 (07/11/2019)

- correct backend flush loop
- test and declare support for Current and LTS node
- Correct reporter decleration in test runner
- Convert codebase from var -> let / const (#673)
- correct npm test script
- correct travis deploy step

## v0.8.2 (04/02/2019)

- update travis npm token
- update dockerfile to latest node-lts
- correct gitter link
- update dockerfile base image to node lts
- Add gitter chat badge
- run tests using python 3.7's pickle rather than 2.x cPickle (#669)

## v0.8.1 (03/13/2019)

- drop StatsD instance from proxy ring in instance of healthcheck failures (#665)
- Add myself (elliot blackburn) to maintainers.md (#666)
- add mysql backend link to docs/backend.md
- Adding myself to MAINTAINERS.
- begin testing on node lts and up
- Added "opencensus-backend"
- correct package.json links to new github organisation
- Update MAINTAINERS.md
- remove meta section of README
- Create MAINTAINERS.md
- Create DCO.txt
- Create CODE_OF_CONDUCT.md
- update README post transfer
- Fixing Markdown formatting
- fix simple typo
- Added StatsdClient Kotlin implementation
- fix formatting on backend interface docs
- Update: ignore files
- removes -q switch
- Fix for failing test on node 0.10
- fix usage of process.EventEmitter
- Add plugin Warp10 to StatsD
- Updated graphite link to read the docs

## v0.8.0 (05/05/2016)
- Modularized injest servers, with support for loading multiple servers
- Added configurable tcp injest server
- Added unix socket injest support
- Added tcp repeater functionality
- Added pickle protocol support to graphite backend
- Added configurable IPv6 and TCP support to proxy
- Added telnet admin interface to proxy
- Multiple variable scoping fixes
- Fixes to flush timer to reduce bucket drift
- Fixes to ruby and java example client code
- Dropped support for node v0.8.x
- Fixed dependency issues for modern node versions
- Updated npm hashring dependency to v3.2.0
- Replaced npm node-syslog dependency with modern-syslog v1.1.2

## v0.7.2 (09/02/2014)
- Fixes to detecting valid packets

## v0.7.1 (02/06/2014)
- move contributing information into CONTRIBUTING.md
- Updates winser to v0.1.6
- examples: python: added efficiency note
- python: examples: fixed doctests for Python 3
- Standardized debian log locations
- Enhancement: consume logger in graphite and repeater backends
- Enhancement: update backend documentation
- Enhancement: inject logger object into backend
- Send STDOUT and STDERR to the appropriate files

## v0.7.0 (12/05/2013)
- added cluster proxy
- measure and graph timestamp generation lag
- added median calculation for timers
- support for top percentiles for timers
- drop support for node v0.6.x
- support for setting the process title
- functionality for optionally omitting stats_counts metrics
- improved functionality to delete counters from the management console
- updates to Debian packaging
- added a clojure example client
- cleaned up the Go example client
- increased test coverage
- documentation updates

## v0.6.0 (03/15/2013)
- added new metric types : sets, gauge deltas, histograms
- added ability to delete idle stats
- added support for configurable namespacing
- added standard Deviation to timers stats (.std)
- added last_flush_time and last_flush_length metrics to graphite backend
- added ipv6 support
- added StatsD repeater backend
- added helper script to decide which timers to sample down
- added Windows service support
- added Scala example
- added support for sampling timers.
- added build testing on node 0.8, 0.9, and 0.10
- fixed broken config file watching.
- fixed for DNS errors from UDP socket
- fixed for TCP client goes away crash.
- removed debugInterval in favor of Console backend debugging
- updated and reorganized Docs
- updated examples scripts
- improved the quality of randomness used for sampling.
- moved  config.js to /lib folder to avoid confusion

## v0.5.0 (07/20/2012)
- add support for logging to syslog
- add basic metrics gathering for StatsD and Graphite backend itself
- several fixes and enhancements for the debian resources
- fixed locale bug in Java client.
- multiple fixes for the Java client

## v0.4.0 (06/29/2012)
- add bin/statsd
- Add CLI bash client example
- documentation updates
- bug fixing, sample_data and data got swapped in Perl client
- fix sampling in the python client
- added sum to all metrics and mean to the total
- changed the way we calculate some metrics by using a cumulative sum as it is more efficient for multiple percentile thresholds
- update README mentioning to preferably use ints as values
- Allow multiple metrics to be passed in one UDP packet delimited by a newline character.
- added console backend
- reformat topkeys log to feature sane key/value pairs

## v0.3.0 (05/16/2012)
- support backends installed from npm
- fix test suite failures

## v0.2.1 (05/14/2012)
- add graphite backend in debian packaging

## v0.2.0 (05/04/2012)
- support for pluggable backends

## v0.1.1 (05/02/2012)
- add gauges type
- percentThreshold also accepts list of percentiles
- base sampling on sampleRate
- updates for debian packaging
- client example updates

## v0.1.0 (02/17/2012)
- initial npm release
