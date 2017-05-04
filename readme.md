# The Sufficiently Parallel Web Tester

## Overview

The SPWT is a platform to allow website front-end tests to be performed in parallel by using layered, isolated instances of the web site being tested.

## Air Gaps and Repeatability

The SPWT runs in one or more air-gapped sets of containers. Any external connections from a set of containers should mark a test or test suite as "unrepeatable" because it relies on external resources.

Pivotal Labs [uses custom Docker files](http://engineering.pivotal.io/post/network-traffic-monitoring-with-containers/) to block external calls. 
