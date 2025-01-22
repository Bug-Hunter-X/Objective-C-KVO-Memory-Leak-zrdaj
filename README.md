# Objective-C KVO Memory Leak

This repository demonstrates a common but subtle memory leak in Objective-C related to Key-Value Observing (KVO).  Failure to remove observers properly can lead to objects being retained beyond their lifecycle.

The `BuggyKVOSample.m` file shows the problematic code.  The `FixedKVOSample.m` file provides the corrected implementation.

**Key Concepts:**
* Key-Value Observing (KVO)
* Memory Management in Objective-C
* `addObserver:forKeyPath:options:context:`
* `removeObserver:forKeyPath:`
* `dealloc` method