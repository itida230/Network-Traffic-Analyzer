This project is a Python-based tool for capturing, storing, and analyzing network traffic in real time. It is designed as a lightweight introduction to packet analysis and network monitoring.

*Features*
- Packet Capture: Uses PyShark to capture live packets from a chosen network interface.
- Data Storage: Saves packet details (source, destination, protocol, length, info) into an SQLite database.
- Traffic Analysis: Uses Pandas to:
1) Detect suspicious packets (e.g., unusually large sizes).
2) Identify the most frequent destinations.
-Modular Design: Separate scripts for capturing, storing, analyzing, and orchestrating the workflow.

*Project Structure*

- capture.py – Captures packets using PyShark.
- database.py – Creates and manages the SQLite database.
- analyze.py – Provides analysis functions using Pandas.
- main.py – Runs the full workflow end to end.
