# Incident Management and Reporting Application (IMRA)

IMRA is a Python application designed to facilitate incident management and reporting. It provides functionalities to report incidents, update their status, and generate reports.

## Installation

No installation is required. Simply download the `IMRA.py` file and run it using Python.

## Usage

To use IMRA, follow these steps:

1. Import the `IMRA` class from `IMRA.py`.
2. Create an instance of the `IMRA` class.
3. Report incidents using the `report_incident` method.
4. Update incident status using the `update_incident` method.
5. Generate reports using the `generate_report` method.

Example usage:

```python
from IMRA import IMRA

# Create an IMRA instance
imra = IMRA()

# Report incidents
incident1 = imra.report_incident("Security breach detected", "High")
incident2 = imra.report_incident("System performance issue", "Medium")

# Update incident status
imra.update_incident(incident1.id, "Investigating", "Investigating potential intrusion attempts")
imra.update_incident(incident2.id, "Resolved", "Restarting service resolved the issue")

# Generate report
imra.generate_report()
