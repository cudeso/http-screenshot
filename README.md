# http-screenshot

* NMAP NSE module to get screenshots of websites
* Uses both wkhtmltoimage and chromium headless

`nmap -p 80,8000 --script http-screenshot -sV 127.0.0.1`

* Outputs
** html-source-nmap-target.html : HTML source
** screenshot-nmap-target.png : screenshot via wkhtmltoimage to png
** screenshot-nmap-chrome-target.pdf : screenshot via Chrome to PDF
** screenshot-nmap-chrome-target.png : screenshot via Chrome to png

* Timing
Sometimes Chrome can stall between different screenshots. Set the nmap timing to a more relaxed scanning.


