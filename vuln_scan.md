---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Vulnerability scans
{{site.data.keyword.BluSoftlayer_full}} partners with Nessus to provide vulnerability scans for any device on the {{site.data.keyword.BluSoftlayer_notm}} network.  Vulnerability scans test for areas of weakness in a device and return a report of the analysis, security issues and fixes for your host device.  Performing vulnerability scans on your devices ensure that they stay secure at all times and are also the first resource to employ when you think a device might be vulnerable or compromised.  Vulnerability scans can be completed using the [Customer Portal ![External link icon](../../icons/launch-glyph.svg "External link icon")](https://control.softlayer.com/) on any device associated with your account.
{:shortdesc}

## Nessus Security Scanner 
{{site.data.keyword.BluSoftlayer_notm}} provides an online security scanner, powered by the open source Nessus Scanning tool. This security scanner can be accessed under the Security tab by clicking on **Scanner**. For more information, see [Nessus Scanning tool ![External link icon](../../icons/launch-glyph.svg "External link icon")](http://www.nessus.org/nessus/).

The **Scanner** page provides a list of hardware available to the Nessus tool hosted by {{site.data.keyword.BluSoftlayer_notm}}. To scan a server, or to see the results of a previous scan, click the details link for the server you wish to inspect. The vulnerability scanning details page shows a short summary of the server (containing the server name, the IP address that to be scanned, and the data center where the server is located.) **Start Scan** schedulea your server with the Nessus scanning server to be vulnerability scanned as soon as possible.

After the server summary is a table of current and past Nessus vulnerability scans. Listed for each scan is the date the scan was requested, the date the scan was started, the status of the scan, and if the scan has completed, a link to the Nessus report.

Nessus reports can have one of these status:

* Scan Pending: The scan has been scheduled for the Nessus scanner box.
* Scan Processing: The scan is currently in progress.
* Generating Report: The scan has completed, and test results are being compiled into a report.
* Scan Complete: The scan successfully completed and the vulnerability report has been generated.
* Scan Cancelled: The Nessus scan was manually canceled by a {{site.data.keyword.BluSoftlayer_notm}} technician.

For all successfully completed Nessus scans listed in this table, a report can be viewed by clicking **View Report**. The report has two tables: a Scan Details table, which lists the number of hosts that were scanned, the number of open security vulnerabilities (holes) found, and the number of possible security vulnerabilities (warnings) found. The second table lists all the security issues found: the host that the vulnerability was found on, and a description of the possible vulnerability.

The open source Nessus tool is plug-in based, which allows new tests to be developed as vulnerabilities are found. {{site.data.keyword.BluSoftlayer_notm}} updates the internal Nessus tool regularly, so regular scanning with the security scanner is recommended to keep up to date with new threats.

For the scan be successful, connections from both 173.192.255.232 and 172.17.19.38 need to be allowed access to your server.
