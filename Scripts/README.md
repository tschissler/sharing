# Scripts
This folder contains several scripts helping with varios tasks.

## TestResultsParser.py
The script is parsing the output of a test run with www.platformio.org and converting it to a NUint testresult XML format (https://github.com/nunit/docs/wiki/Test-Result-XML-Format).
I used this scriprt to upload the test results while running a Azure DevOps Build Pipeline.

You can use this command to create a file to be parsed:

<code>pio test >> testresults.txt</code>

And then parse it with
<code>TestResultsParser.py testresults.txt testresults.xml</code>
