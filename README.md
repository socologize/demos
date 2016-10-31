# demos
Prototype Demo Code for security community


# Volatize.py
An automation tool for the Volatility Memory Forensics Framework. Focused on analysis productivity.
Current DEMO CODE works on Python 2.7.x

______________________________________________________________________
 Volatility Foundation (c) - An advanced  memory forensics framework
______________________________________________________________________

 Volatize.py By The Foundstone IR Group - Volatility Automation Tool

	     Demo Version: GitHub://
_____________________________________________________________________


# Dependencies
You need the following packages installed to use Volatize
- requests  : pip install requests
- tabulate  : pip install tabulate
- futures   : pip install futures
- tqdm      : pip install tqdm
- Volatility

# Why Volatize
Intended to maximize productivity when analyzing memdumps.  I saved 71 minutes of just typing and waiting for output from the plugins I would run. Also, the concept of playbooks left unattended as visio diagrams and hard to manage scripts are an ineffective way to lead robust security operations. The usage of Volatize is intended to fix this by digitizing your visios, processes, or notes into a digital playbook for memory forensics.  

All tactical teams benefit by trying to digitize the playbooks they have within their orgs with tools like Volatize.  If you do not have the in-house expertise, reach out to me (us) and we will gladly help add your playbooks to the tool.  

# Are there other tools already?
While many great researchers are developing Flask, Django or other forms of automated tools, I am focusing on lightweight CLI workflows. 

Kudos to the authors of such tools like vortessence, volutility, volatility-bot, etc.!

# How To Run?
if you have a memory sample and want to run in automode:

>>> $ volatize.py parsemem --auto --memory "path/to/memory/sample"

Or if you just want to setup the case structure to parse memory:

>>> $ volatize.py parsemem --setup --memory "path/to/memory/sample"

# Quick Explanation on Profile Independent Automation
[![VOLATIZE DEMO](https://lh3.googleusercontent.com/oJZCPKaa0w8_TVtb90JL-yUOPNCR1qcIq3PXRwVpZtSUYS-wJnK6LvvcUrHJ0Ve5WuhYng=s152)](https://www.youtube.com/watch?v=dWQ_tNAnKXA, "Volatize Auto")

# How To Use the VOLCASE Structure?
VOLCASE is a small script that organizes a set of folders to keep you productive and organized in your own workflow.
The case structure and its synopsis is:

______________________________________________________________________
           Case Structure for Memory Analysis

              BULKEX  :  Dump BulkExtractor Output
               DUMPS  :  Dump PIDS, DLLS, etc.
             PLUGINS  :  Dump Volatility Plugins Output
           PROFILING  :  Dump Special Profiling Items
             STRINGS  :  Dump Strings Utility Output
           TIMELINES  :  Dump Body Format Output
                VADS  :  Dump VADS from PIDS
           YARASCANS  :  Dump Yarascan Output

______________________________________________________________________



When you run volatize.py in "--auto" or "--parse" mode, the Volatility plugins will save text files under the PLUGINS folder.
_______________________________________________________________________
 PLUGINS/
	 -> amcache.text
	 -> atoms.text
	 -> atomscan.text
	 -> auditpol.text
	 -> callbacks.text
	 -> clipboard.text
_______________________________________________________________________


# Recognition
@aboutsecurity from Foundstone Intel Security Group on 'Fit for Purpose' feedback
@rwgresham from Foundstone Intel Security Group on Bash prototypes for automation
@jx212fs from Foundstone Intel Security Group on code refinement and 'can-do' attitude
