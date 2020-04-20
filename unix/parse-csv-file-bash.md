# Parse a CSV File in Bash

You can parse the contents of a comma-separated value (CSV) file in a Bash
script by using the `read` command. You must first set the input field separator
to a comma to separate the individual fields by setting `IFS=','`. You can then
call the `read` command in a loop to parse each line of input and store its
fields in a set of variables.

```bash
#! /usr/bin/env bash
IFS=','
INPUT=foo.csv
while read field1 field2 field3 field4
do
    echo "Field 1: $field1"
    echo "Field 2: $field2"
    echo "Field 3: $field3"
    echo "Field 4: $field4"
done < $INPUT
```

It is good practice in a production script to store off the original value of
`IFS` and restore it after parsing the data.
