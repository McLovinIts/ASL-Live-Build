# ASL-Live-Build Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.0.0-beta.2] - 2021-02-05

- Add Supermon by default
- Add Allmon2
- Armhf fixes
- Use live-build hooks instead of scripts so PC and Pi can have parity
- Use systemd service instead of init.d service
- Refactoring of build scripts

## [2.0.0-beta] - 2021-01-31

What’s new in ASL 2.0.0-beta?

- Runs on Raspberry Pi 2, 3 and 4 as well as Intel-AMD.
- One OS and code base across all platforms.
- Survives kernel updates.
- New cli> command rpt lookup <node#> (ala HamVoIP) to resolve IP address of any node.
- Most of the C code has been refactored to compile with current compiler.
- Http registration with failover to IAX2.
- Multi-thread
- Use libcurl for statpost instead of shell call to wget
- Update startup/shutdown scripts to query systemctl for service status
- Clean up output from cli>rpt local nodes
- Updates to asterisk service management convenience scripts
- Fix compiler warnings, perhaps better system stability
- Collect perceived ip, port and refresh time from http registration
- Add libi2c-dev to list of build dependencies
- Add registerhttp and registeriax directives to chan_iax2
- Inclusion of systemd service file for updatenodelist
- Implementation of console command rpt lookup
- Fix ASTDATADIR location
- Implement http(s) registration
- Include app_rpt in the build package
- Merge in telemetry ducking
- Merge in upstream alignment
- Merge in simple voter
- Merge in http registration
- Change naming convention to asl-asterisk
- Depend on new asl-dahdi packages
- Compile with modern gcc
- Repackage various AllStar pieces into new Debian packages
