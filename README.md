A simple PowerShell script to keep Remote Desktop Protocol (RDP) sessions alive by simulating periodic Shift key presses.
Purpose

In some environments, idle RDP sessions are disconnected automatically due to inactivity.
This script helps maintain active sessions by programmatically simulating key presses at set intervals.
Features

    Customizable interval between simulated key presses

    Optional timer for how long the script should run

    Console output for visibility during operation

Usage

Open PowerShell, navigate to the script directory, and run:

.\keepalive.ps1

Run with a custom interval (in seconds) and duration (in minutes)

.\keepalive.ps1 -Interval 180 -Duration 60
Parameters
Parameter	Description	Default
Interval	Interval in seconds between simulated key presses	240
Duration	Total duration in minutes to run the script (-1 for infinite)	-1
Example

Run the script with a 3-minute interval for 1 hour:

.\keepalive.ps1 -Interval 180 -Duration 60
Disclaimer

Use responsibly.
This script is intended for environments where you have permission to prevent session timeouts. Unauthorized use in restricted environments may violate IT policies.

