YoPy
====

A simple Yo! API for python.

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
Here is a Python 2 example :

	import yopy

	token = <your_api_token>
	username = "PARTHDHAR"
	link = "https://github.com/parthanium/YoPy"

	yo = yopy.Yo(token)
	print yo.number()
	yo.yoall(link)
	yo.youser(username, link)

Parth Dhar<br/>
2014
