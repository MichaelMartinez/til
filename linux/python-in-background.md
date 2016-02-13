# Run Python script as background process

_Ubuntu_

1. Be sure the script points to the correct env with hash bang `#! /path/to/env`
2. Make the script executable `chmod +x`
3. Start the script: `nohup /path/to/script.py &`
4. To search for the PID of the process: `pgrep script.py`
5. To kill the script use PID from previous step: `kill <PID>`
