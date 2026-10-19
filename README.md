# ChatApp

A multi-client chat room in Python using TCP sockets and threads, with a Tkinter GUI. Written in 2025 as a networking exercise.

- **Server** (`server.py`): accepts clients on a TCP port, runs one thread per connection, and broadcasts each message to every other client.
- **Client** (`client.py`): separate send and receive threads, so the GUI never blocks; a Tkinter window with a message list and an input box. Type `QUIT` to leave.

## Run

```bash
python3 server.py localhost -p 1060
python3 client.py localhost -p 1060   # start one per user
```

Needs Python 3 with Tkinter (standard library).
