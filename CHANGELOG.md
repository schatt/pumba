# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [0.1.5] - 2016-04-13
### Added
- File: `pumba_kube.yml` Kubernetes (1.1.x) deployment manifest
- File: `pumba_coreos.service` CoreOS `fleet` service file
- Flag: `--json` flag. When specified log will be generated in JSON format (Logstash and Splunk friendly)
- Flag: `--slackhook` Slack web hook URL. Now Pumba can report log events to specified Slack channel.
- Flag: `--slackchannel` Slack channel to report Pumba events in.
- Flag: `--dry` enable 'dry run' mode: do not 'kill' containers, just log intention
### Changed
- by default produce colarful log to TTY
### Fixed
- fix failure when container name is empty (all containers)

## [0.1.4] - 2016-04-08
This is initial release of Pumba Docker Chaos Testing
### Added
- `run` command
- `--random` option: randomly select matching image to "kill"