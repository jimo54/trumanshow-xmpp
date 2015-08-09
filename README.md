# trumanshow-xmpp

The included files provide for (semi-)autonomous chat bots for BetaPort.

* buddylist.py -- This is a script to create rosters (buddy lists) for the chat bots. The current version works only with the Python 2 xmpp library. **Needs updating for Python 3.**

* Python 3 version:
** chatagent3.py -- The Python 3 ChatAgent class. Works well with Prosody servers. Note the requirements included in comments at the top of the file.
** testagent3.py -- The driver script for chatagent3.py. The Python 3 version spawns child processes (rather than threads) for the agents. This change was necessitated by the fact that the sleekxmpp client is itself threaded.

* Python 2 version:
** chatagent_home.py -- The Python 2 ChatAgent class. Works well with Prosody servers. Note the requirements included in comments at the top of the file.

** testagent_home.py -- The driver script for chatagent_home.py.

* prosody.cfg.lua -- Example prosody config file.