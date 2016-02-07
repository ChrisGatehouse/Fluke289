# Fluke289

This is a very basic library to access values from your Fluke287/289.

UsaveExample:

```python

from Fluke289 import Fluke289

portName = "/dev/ttyUSB2"

f = Fluke289(portName)
f.id()
#f.defaultSetup()
print f.queryPrimaryMeasurement()
print f.value()

while True:
	print f.value()

```
