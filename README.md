# test-machine

A library for testing kafka applications

This library was originally part of jackdaw but I have extracted it out
so that folks can depend on one without the other. This helps in
scenarios like...

 1. A user of jackdaw does not wish to pull in additional dependencies
    required only by the test-machine like aleph or the kafka admin
		client

 2. A user of the test-machine has a kafka based system implemented
    using something other than jackdaw (e.g.

     - a bunch of kafka-connect jobs,
		 - streams defined in KSQL
		 - a kafka streams application defined using plain old java
		 
In addition, the test-machine has not been available as part of jackdaw
since April 2020 when the code for it was [moved](https://github.com/FundingCircle/jackdaw/pull/235)
under the `test/` directory and consequently not available to folks that depend
on it.

I have not yet re-constituted the docs but the docs in jackdaw are
still applicable for now. There is both a
[guide](https://cljdoc.org/d/fundingcircle/jackdaw/0.7.6/doc/the-test-machine)
to the library that explains at a high-level how it works and how to use
it, and [reference
documentation](https://cljdoc.org/d/fundingcircle/jackdaw/0.7.6/api/jackdaw.test)
for the individual docstrings.

## License

Copyright © 2020 Andy Chambers

Distributed under the Eclipse Public License either version 1.0 or (at
your option) any later version.
