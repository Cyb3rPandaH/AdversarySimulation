# Python Execution via WhatsApp

* Author: Jose Rodriguez - [@Cyb3rPandaH](https://x.com/Cyb3rPandaH)

## Description

Inspired by an article from [Bleeping Computer](https://www.bleepingcomputer.com/news/security/whatsapp-for-windows-lets-python-php-scripts-execute-with-no-warning/), we decided to test the execution of Python scripts using the WhatsApp desktop application.

According to the article, the WhatsApp client does not block from launching: .PYZ (Python ZIP app), .PYZW (PyInstaller program), and .EVTX (Windows event Log file).

They also confirmed that WhatsApp does not block the execution of Python files and discovered that the same happens with PHP scripts.

The behavior was tested on both Windows 10 and Windows 11 systems.

## Simulation

We decided to test the execution of Python scripts using the WhatsApp Desktp application.

### Virtual Machines

* Attacker machine: Kali Linux 2023.4
* Victims machine: Windows 10 - Version 22H2 - OS Build 19045.4651

### Scenarios

* Execution of **.py** file: With Virus & Threat protection enabled, WhatsApp application blocked execution.
* Execution of **.pyz** file: With Virus & Threat protection enabled, WhatsApp application blocked execution, but Windows Security blocked the execution.
* Execution of **.pyz** file: With Virus & Threat protection disabled, WhatsApp application did not blocked execution, and we got a meterpreter session on Kali Linux system.

### Video recording

You can find a video recording of the simulation [here](https://youtu.be/T05vXpZXFJY?feature=shared).
