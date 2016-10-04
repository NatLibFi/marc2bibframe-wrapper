# marc2bibframe-wrapper
Java wrapper for the Library of Congress [marc2bibframe](https://github.com/lcnetdev/marc2bibframe) conversion utility, heavily based on a [wrapper script](https://gist.github.com/kefo/10416746) by Kevin Ford. The features are the same, but the script has been updated to work with the latest marc2bibframe XQuery conversions and wrapped in an Eclipse/Maven project for easier maintenance and deployment.

Also inspired by, but not directly based on, [ModBibFrame](https://github.com/jgreben/ModBibFrame) by Joshua Greben, which has some additional features such as conversion starting from MARC21 binary format records, URI rewriting and looking up authorities in a database.

This utility allows running the marc2bibframe utility on large batches of records at a time. Internally, records are processed one at a time and a conversion error in a single record will not stop the whole conversion. Errors are logged in an XML log file that also includes the MARCXML data of problematic records.

# License

There was no license information attached to the gist that this code is based on, but the marc2bibframe code [is in the public domain](https://github.com/lcnetdev/marc2bibframe/blob/master/LICENSE.txt) as it's developed by the Library of Congress, so the same license (or lack thereof) probably applies for the wrapper as well.