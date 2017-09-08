**webkit2png** 
==============

About
------
Python script that takes screenshots (browsershots) using webkit

##Installation
Ubuntu (Terminal)
------
- Add following packages: ``apt-get install python-qt4 libqt4-webkit xvfb``
- Install the flash plugin to screenshot Adobe Flash files: ``apt-get install flashplugin-installer``
- Clone project via git

Usage
=====
- For help run: ``python webkit2png/scripts.py -h``
- For rendering run: ``python webkit2png/scripts.py http://www.google.de -x 1280 1200 --output=screenshot.png``


REMARK: At present there is no user agent selection available. To enable this you could add the following method (overriding the super class QWebPage method):
``def userAgentForUrl(self, url): return QString("Mozilla/5.0 (iPhone; CPU iPhone OS 10_3 like Mac OS X) AppleWebKit/602.1.50 (KHTML, like Gecko) CriOS/56.0.2924.75 Mobile/14E5239e Safari/602.1")``
