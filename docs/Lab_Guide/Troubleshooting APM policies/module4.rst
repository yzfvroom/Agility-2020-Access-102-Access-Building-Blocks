Lab 4: Troubleshooting
======================

Welcome to the troubleshooting APM Policies lab.  This lab is optional.
The lab exercises will provide guidance on how to configure and troubleshoot
common Access Policy Manager (APM) issues as experienced by field engineers,
support engineers, and customers.  This guide is intended to complement 
lecture material provided during the course as well as reference guide for 
students after the class as a basis for troubleshooting APM within your
own environment.


Task 1: Jump Host
----------------------

#. Establish an RDP connection to your Jump Host as well as login to the GUI
of the bigip1.f5lab.local BIG-IP system.

Task 2: General Troubleshooting
------------------------
 
In this lab exercise, you will learn where to look and what to look at when an Access Policy 
is not successfully allowing access or not performing as intended.

# Questions to ask yourself

# Do we have proper Network Connectivity?

# Are there any Upstream/Downstream Firewall Rules preventing APM to be reachable or to reach destination
targets it requires to access?

# Do we have DNS setup properly?

# Do we have NTP setup properly?

# Are we receiving any Warnings or Error messages when we logon?

# Are there any missing dependencies?

# Time to check on our Sessions under Manage Session Menu

    # What can we see from the Manage Session Menu?
    # If we click the Session ID link what more information is available?
    # Is Authentication Successful or is it Failing?
    # Is the user receiving the proper ENDING ALLOW from the Policy?
	
# Time to Review the Reports information for the Session in question

    # What information is available from the ALL SESSIONS REPORT?
    # Can we review the Session Variables for the user’s session from the ALL SESSION REPORT? If YES then Why however If NO then WHY?

# Can the BIG-IP TMOS Resolve the AAA server by Hostname and by Hostname.Domain?

    # Is the AAA reachable over the network, no Firewalls blocking communication from BIGIP Self-IP?

# Manage Sessions within the Access Policy Manager menu

# We use the Manage Sessions menu to view general status of currently logged in sessions,
view their progress through a policy, and to kill sessions when needed.

# Open a USER session to APM through a new browser window by navigating to your first Virtual
Server IP Address created in LAB I 

# Did you receive an error message? If so, take note of the Session Reference Number

# In the browser window, you are using to manage the BIG-IP, navigate to Access  Overview > Active Sessions menu.

# Review the Manage Sessions screen, is there an Active Session? If not then why?





