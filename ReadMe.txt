Introduction

• The Hypercheck tool is a utility to perform pro-active self checks on Hyperflex clusters to ensure its stability and resiliency.
• It also helps perform automated pre-upgrade checks to have a better upgrade experience.
• The tool automates a list of checks on Hyperflex System saving time during Maintenance activity and Upgrade processes.

NOTE: Always download latest version of the tool before you use it. Since the tool is enhanced frequently, using older version may result in missing important checks.

Supported HX Versions
    1.8
    2.0
    2.1
    2.5
    2.6
    3.0
    3.5
    4.0

Supported HX Clusters
    Hyperflex Standard Cluster
    Hyperflex Edge Cluster (2Node, 3Node and 4Node)
    Only supported on Hyperflex cluster on VMWare ESXi

When to use?
    Before Hyperflex upgrades.
    Hyperflex Health Check before and after Maintenance Windows
    When working with Cisco TAC
    Pro-active Health Check anytime.

How to use the tool?
Pre-requisite:  Script needs HX and ESXI root password information to check all conditions

Steps:
1) In GitHub, click on the “Clone or download” button and choose the “Download ZIP” option. This will download a file titled “Hyperflex-Hypercheck-master.zip”
2) Upload Hyperflex-Hypercheck-master.zip to the SCVM (preferably HX Cluster Management IP).
3) unzip the Hyperflex-Hypercheck-master.zip (#unzip Hyperflex-Hypercheck-master.zip)
4) Change directory to Hyperflex-Hypercheck-master (# cd Hyperflex-Hypercheck-master)
5) Now run the python script file with below command:
   a) For Test summary report:
      python HXTool.py
   b) For Test detail report:
      python HXTool.py detail
6) Enter the HX root password.
7) Enter the ESXi root password.
8) Script will display the result on the console and also creates each node report(HX Report 10.X.X.79.txt) and main report txt file(HX Tool Main Report.txt) in the HX_Report_<timestamp> folder.

Test Details:
Detail info of the test are available in the file(TestInfo.txt).

For stopping the script execution we can use the key [CTRL+Z] 

Refer the following for more information on Hypercheck Tool-
https://www.cisco.com/c/en/us/support/docs/hyperconverged-infrastructure/hyperflex-hx-data-platform/214101-hypercheck-hyperflex-health-pre-upgr.html

