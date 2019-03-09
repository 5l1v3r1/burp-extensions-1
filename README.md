# Burp Extensions
A collection of scripts to extend Burp Suite. Most are just sample scripts that interact with Burp in a particular way, mainly to demonstrate how to interact with Burp. The code is commented well enough (hopefully!) to follow.

Step-by-step tutorials to write Python extensions:

https://laconicwolf.com/2019/03/09/burp-extension-python-tutorial-generate-a-forced-browsing-wordlist/
https://laconicwolf.com/2019/02/07/burp-extension-python-tutorial-encode-decode-hash/
https://laconicwolf.com/2018/04/13/burp-extension-python-tutorial/

## Extensions

### GenerateForcedBrowseWordlist.py
Extracts the filenames from URLs in scope or from a selected host. Just right click on the hosts pane in the sitemap and click 'Generate forced browsing wordlist' for either selected items or all hosts in scope. The output will appear in the extender tab, where you can set configure the extension to output to the system console, save to a file, or show in the UI.

### ExampleRepeater.py
Like repeater, only without any of the features, bug checking, or elegance. A simple example that creates a tab with a split-panel GUI, where the top pane can be populated (By right-clicking and 'Send to ...' or just typing it) with an HTTP request. It implements a button, that when clicked, sends the HTTP request and writes the response to the bottom pane.

### RequestAsPython-PowerShell.py
Once again, extensions already exist for this, but is an example of a tab with a split panel GUI. Top pane is for an HTTP request, and the bottom pane contains a button and three text fields. Click the button, and the request gets transformed to its equivalent in Python requests, Python urllib2, and PowerShell Invoke-WebRequest. Not all methods and use cases were tested, but seems to work okay.

### encodeDecodeHash.py
Performs encoding, decoding, and hashing similar to ZAP's encode/decode/hash tool. 
