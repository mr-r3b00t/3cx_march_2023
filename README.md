# 3cx_march_2023

Forked with love by R3.

IOC searches with artifacts provided by SentinelOne
https://www.sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/


- device_file_events.kql - Searches hashes across DeviceFileEvents, DeviceImageLoadEvents, DeviceNetworkEvents. 
- mde_hunting.kql - Pulls domain IOC list from domains.txt and searches accross DeviceNetworkEvents, DeviceFileEvents, DeviceEvents. Dan/mr-r3b00t/@UK_Daniel_Card
- process_network_events.kql - searches for 3CXDesktopApp.exe across DeviceNetworkEvents. Created by Dan/mr-r3b00t/@UK_Daniel_Card


Thank you to Dan/mr-r3b00t/@UK_Daniel_Card for putting these together in the first place.