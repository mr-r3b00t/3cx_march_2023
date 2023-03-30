# 3cx_march_2023

Forked with love by R3.

## News and Updates

- IOC searches with artifacts provided by SentinelOne
https://www.sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/

- Update from CS:
https://reddit.com/r/crowdstrike/comments/125r3uu/20230329_situational_awareness_crowdstrike/

- Thread from 3CX
Initial: https://3cx.com/community/threads/threat-alerts-from-sentinelone-for-desktop-update-initiated-from-desktop-client.119806/page-5
Dedicated: https://3cx.com/community/threads/3cx-desktopapp-security-alert.119951/

Blogs
https://sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/
https://crowdstrike.com/blog/crowdstri

## File list

- device_file_events.kql - Searches hashes across DeviceFileEvents, DeviceImageLoadEvents, DeviceNetworkEvents. Created by R3 SecOPs Team.
- mde_hunting.kql - Pulls domain IOC list from domains.txt and searches accross DeviceNetworkEvents, DeviceFileEvents, DeviceEvents. Created by Dan/mr-r3b00t/@UK_Daniel_Card
- process_network_events.kql - searches for 3CXDesktopApp.exe across DeviceNetworkEvents. Created by Dan/mr-r3b00t/@UK_Daniel_Card
- domains.txt contains list of domains seen as IOCs published by SentinelOne
- hashes.txt contains list of hashes SentinelOne

## Looking for other detection content?

Thank you to https://twitter.com/Sam0x90 for compiling this list:

Samples:
https://share.vx-underground.org/SmoothOperator.7z

MacOS sample analysis:
https://twitter.com/patrickwardle/status/1641294247877021696



## Thanks to

- Dan/mr-r3b00t/@UK_Daniel_Card for putting these together in the first place.
- https://twitter.com/Sam0x90 for compiling a list of resources.