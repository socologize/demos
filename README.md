# demos
Prototype Demo Code


# Volatize.py
An automation tool for the Volatility Memory Forensics Framework. Focused on analysis productivity.
Current DEMO CODE works on Python 2.7.x

# Dependencies
You need the following packages installed to use Volatize
- requests  : pip install requests
- tabulate  : pip install tabulate
- futures   : pip install futures
- tqdm      : pip install tqdm
- Volatility

# Why Volatize
Intended to maximize productivity when analyzing memdumps.  I saved 71 minutes of just typing and waiting for output from the plugins I would run. Also, the concepts of playbooks being just visio diagrams and heard to manage scripts are a great benefit for those seeking to to digitize the playbooks they have within their orgs.  

While many great researchers are developing Flask, Django or other forms of automated tools, I am focusing on lightweight CLI workflows. Kudos to the authors of such tools.

# How To Run?
if you have a memory sample and want to run in automode:

>>> $ volatize.py parsemem --auto --memory "path/to/memory/sample"

Or if you just want to setup the case structure to parse memory:

>>> $ volatize.py parsemem --setup --memory "path/to/memory/sample"

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
