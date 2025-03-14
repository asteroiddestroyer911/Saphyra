# Saphyra: A HTTP Request Flooder


Saphyra is a lightweight Python script designed to perform HTTP request flooding against a specified target URL. This tool is primarily intended for educational purposes, such as stress testing your own web applications or understanding the impact of high traffic on server performance.


## Features:


• Multi-threaded Requests: Utilizes threading to send multiple requests simultaneously, simulating high traffic.

• Randomized User Agents: Randomly selects from a list of user agents to mimic different browsers and reduce detection.

• Dynamic Referers: Generates random referer URLs to further obfuscate the source of the requests.

• Delay Handling: Implements random delays between requests to avoid triggering rate limits and bans.

• Error Handling: Catches HTTP errors and adjusts behavior based on server responses (e.g., handling 429 Too Many Requests).

• Monitoring: Provides real-time feedback on the number of requests sent during the operation.


## Usage:

To run Saphyra, use the following command (using bash) :

```bash
python Saphyra.py <url> <port>
```

Replace <url> with the target URL (must start with http:// or https://).

Optionally specify <port> (default is 80).


## Requirements:

1. Python 3.x

2. urllib library (included in standard Python library)
