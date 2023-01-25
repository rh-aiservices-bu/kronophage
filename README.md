# kronophage

> The project that eats time for breakfast!

## Goals

A more fine-tuned control of the scaling related to running notebook pods on OpenShift

## Features

* Notebook Images Pre-Puller
  * A daemonset that automatically caches (some or all) images on (some or all) nodes.
  * Ideally, choose all current RHODS images + custom images by default
* Notebook Nightly Killer
  * asks KFNBC to stop all notebook pods at midnight (or the time of your choosing)
  * include all RHODS notebooks in all namespaces
* Cluster Stretcher
  * allows to create arbitrary virtual users to pre-grow the cluster
  * manually change replicas from 0 -> 200 -> 0
  * these pods needs to be preemptible
* Cluster Stretcher Scheduler
  * Allows to change the # of replicas of the cluster stretcher at certain times
  * e.g. set it to 200 at 8:30 am on mondays, set it to 2 at 9:01 on mondays

## Usage

* Each of these 4 things can be turned on (default) or off
* Some have variables (e.g "killing_time") with default values (e.g "3 am")

## Implementation



## Removal


## Design

Design notes are stored [here](DESIGN.md)