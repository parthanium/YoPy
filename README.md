YoPy
====

Python wrapper for the Yo! API

As of now, you can:
<ol>
	<li>Get the number of subscribers</li>
	<li>Send a Yo! to all subscribers</li>
	<li>Send a Yo! to a specific user</li>
</ol>

YoPy requires a Yo! API access token. You can get one by registering at http://dev.justyo.co/

Dependencies
============
YoPy requires the module Requests. Get it from http://docs.python-requests.org/

Installation
============
To install, simple copy <code>yopy.py</code> to the <code>Lib</code> folder of your Python installation.

Usage
=====
YoPy works with any version of Python, as long as it supports Requests.<br/>
can only send link OR location but not both) format: lat,long<br/>
Here is a Python 2 example :

	import yopy

	token = <your_api_token>
	username = "PARTHDHAR"
	link = "https://github.com/parthanium/YoPy"
	location = "41.0256377,28.9719802"

	yo = yopy.Yo(token)
	print yo.number()
	yo.yoall(link=link)
	yo.yoall(location=location)
	yo.youser(username, link=link)
	yo.youser(username, location=location)

Parth Dhar<br/>
2014


[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/parthanium/yopy/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
