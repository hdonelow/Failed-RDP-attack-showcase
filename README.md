# Failed-RDP-attack-showcase
 This GitHub repository features a PowerShell script designed to extract information from Windows Event Logs pertaining to failed RDP attacks. The script further leverages a third-party API, specifically ipgeolocation.io, to retrieve geographic details about the attackers.


In the provided demonstration, I showcase the utilization of this script in conjunction with the setup of Azure Sentinel (SIEM). The demonstration involves the connection to a live virtual machine functioning as a honeypot, enabling real-time observation of global RDP brute force attacks. The custom PowerShell script is then employed to query the attackers' geolocation information, which is subsequently visualized on an Azure Sentinel Map.


Key Features:

PowerShell script for extracting RDP failed logon logs from Windows Event Viewer.
Integration with ipgeolocation.io API for obtaining geographic data based on IP addresses.

Demonstration Setup:

1. Azure Sentinel (SIEM) deployment.
2. Connection to a live virtual machine acting as a honeypot for observing global RDP brute force attacks.

Execution Flow:

1. Detection of RDP event fail logs in Windows Event Viewer.
2. Utilization of ipgeolocation.io API to fetch geographic information associated with attacker IP addresses.
3. Custom logs generation, including geodata.
4. Visualization of incoming attacks on a world map within Azure Sentinel after 24 hours.

Notable Points:

Specifically tailored for RDP brute force attacks.
Geographic information provides insights into the global origin of the attacks.
Custom logs enhance the tracking and analysis of attack patterns.
This project aims to enhance situational awareness by correlating RDP attack data with geographic details, ultimately contributing to a comprehensive understanding of the threat landscape.
