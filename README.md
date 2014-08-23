nsi-docker-kibana
=================

*Node.js Services Integration - Docker image for elasticsearch/kibana based on docker-passenger*

This image contains a bare install of [elasticsearch](http://www.elasticsearch.org/) and [kibana](http://www.elasticsearch.org/overview/kibana/).

Inspired by the [public elasticsearch trusted build](https://github.com/dockerfile/elasticsearch).

It is based on [docker-passenger](https://github.com/phusion/passenger-docker) for nodejs even if it doesn't use phusion passenger or node.js itself. This is because it is made to serve as a base for containers that will use these tools.

Install
-------

    docker pull albanm/nsi-kibana

Usage
-----

    docker run -d -p 9200:9200 -p 9300:9300 -v <data-dir>:/data albanm/nsi-kibana
