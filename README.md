An example of Unity 3D 2017 works with ZeroMQ
=============================================

### Environment

Unity 2018.2.5f1

Python 3.6.0

Tested on Windows 10

### What's in this demo

Python scripts:

- a_in_scan_foreground (acts as server collecting mcdaq data)

C# scripts:

- [client](Assets/ClientObject.cs) (in a PUB/SUB model)
- [server](Assets/ServerObject.cs) (in a REQ/REP model)

Scene:

- [Main demo scene](Assets/main.unity)

### How to run

First start 2 python scripts (in seperate shell sessions):

```bash
python3 a_in_scan_foreground.py
```

Then start play mode of main demo scene in Unity Editor.

You should see the box move around according to values measured by the mccdaq.
