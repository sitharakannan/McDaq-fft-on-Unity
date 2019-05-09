Communication between Unity and MCcDaq
=============================================

### Setup

Please follow the installation instructions from the README of: https://github.com/mccdaq/mcculw

### Environment

Unity 2018.2.5f1

Python 3.6.0

Tested on Windows 10

### What's in this demo

Python scripts:

Inside Python folder:
- background_file (acts as server collecting mcdaq data)
Press ctrl-c to stop collecting data

C# scripts:

- [client](Assets/ClientObject.cs) (in a PUB/SUB model)

Scene:
- [Main demo scene](Assets/main.unity)

### How to run

First start python script:

```bash
python3 background_file.py
```

Then start play mode of main demo scene in Unity Editor.

You should see the box move around according to values measured by the mccdaq.
