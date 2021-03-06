<!-- AUTOGENERATED BY glean_parser.  DO NOT EDIT. -->

# Metrics
This document enumerates the metrics collected by this project using the [Glean SDK](https://mozilla.github.io/glean/book/index.html).
This project may depend on other projects which also collect metrics.
This means you might have to go searching through the dependency tree to get a full picture of everything collected by this project.

# Pings

 - [metrics](#metrics)


## metrics

This is a built-in ping that is assembled out of the box by the Glean SDK.

See the Glean SDK documentation for the [`metrics` ping](https://mozilla.github.io/glean/book/user/pings/metrics.html).

The following metrics are added to the ping:

| Name | Type | Description | Data reviews | Extras | Expiration | [Data Sensitivity](https://wiki.mozilla.org/Firefox/Data_Collection) |
| --- | --- | --- | --- | --- | --- | --- |
| places_manager.read_query_count |[counter](https://mozilla.github.io/glean/book/user/metrics/counter.html) |The total number of read operations performed on the places store. The count only includes operations triggered by the application, not e.g. incidental reads performed as part of a sync. It is intended to be used together with `read_query_error_count` to measure the overall error rate of read operations on the places store.  |[1](https://bugzilla.mozilla.org/show_bug.cgi?id=1607621), [2](https://bugzilla.mozilla.org/show_bug.cgi?id=1649044), [3](https://bugzilla.mozilla.org/show_bug.cgi?id=1694316)||never |2 |
| places_manager.read_query_error_count |[labeled_counter](https://mozilla.github.io/glean/book/user/metrics/labeled_counters.html) |The total number of errors encountered during read operations on the places store, labeled by type. It is intended to be used together with `read_query_count` to measure the overall error rate of read operations on the places store.  |[1](https://bugzilla.mozilla.org/show_bug.cgi?id=1607621), [2](https://bugzilla.mozilla.org/show_bug.cgi?id=1649044), [3](https://bugzilla.mozilla.org/show_bug.cgi?id=1694316)|<ul><li>url_parse_failed</li><li>operation_interrupted</li></ul>|never |2 |
| places_manager.write_query_count |[counter](https://mozilla.github.io/glean/book/user/metrics/counter.html) |The total number of write operations performed on the places store. The count only includes operations triggered by the application, not e.g. incidental writes performed as part of a sync. It is intended to be used together with `write_query_error_count` to measure the overall error rate of write operations on the places store.  |[1](https://bugzilla.mozilla.org/show_bug.cgi?id=1607621), [2](https://bugzilla.mozilla.org/show_bug.cgi?id=1649044), [3](https://bugzilla.mozilla.org/show_bug.cgi?id=1694316)||never |2 |
| places_manager.write_query_error_count |[labeled_counter](https://mozilla.github.io/glean/book/user/metrics/labeled_counters.html) |The total number of errors encountered during write operations on the places store, labeled by type. It is intended to be used together with `write_query_count` to measure the overall error rate of write operations on the places store.  |[1](https://bugzilla.mozilla.org/show_bug.cgi?id=1607621), [2](https://bugzilla.mozilla.org/show_bug.cgi?id=1649044), [3](https://bugzilla.mozilla.org/show_bug.cgi?id=1694316)|<ul><li>url_parse_failed</li><li>invalid_bookmark_update</li><li>invalid_parent</li><li>unknown_bookmark_item</li><li>url_too_long</li><li>cannot_update_root</li></ul>|never |2 |


Data categories are [defined here](https://wiki.mozilla.org/Firefox/Data_Collection).

<!-- AUTOGENERATED BY glean_parser.  DO NOT EDIT. -->

