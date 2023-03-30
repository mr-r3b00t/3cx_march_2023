# 3CX March 2023 - KQL Rules and Resource List

Forked with love by R3.

## News and Updates

### IOC searches with artifacts provided by SentinelOne and Sophos
https://www.sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/
https://github.com/sophoslabs/IoCs/blob/master/3CX%20IoCs%202023-03.csv

### Update from CS:
https://reddit.com/r/crowdstrike/comments/125r3uu/20230329_situational_awareness_crowdstrike/

### Thread from 3CX

- `Initial:` https://3cx.com/community/threads/threat-alerts-from-sentinelone-for-desktop-update-initiated-from-desktop-client.119806/page-5

- `Dedicated:` https://3cx.com/community/threads/3cx-desktopapp-security-alert.119951/

## Blogs
- https://sentinelone.com/blog/smoothoperator-ongoing-campaign-trojanizes-3cx-software-in-software-supply-chain-attack/
- https://www.crowdstrike.com/blog/crowdstrike-detects-and-prevents-active-intrusion-campaign-targeting-3cxdesktopapp-customers/

## File list

`device_file_events.kql` - Searches hashes across DeviceFileEvents, DeviceImageLoadEvents, DeviceNetworkEvents. Created by R3 SecOPs Team.

`mde_hunting.kql` - Pulls domain IOC list from domains.txt and searches accross DeviceNetworkEvents, DeviceFileEvents, DeviceEvents. Created by Dan/mr-r3b00t/@UK_Daniel_Card

`process_network_events.kql` - searches for 3CXDesktopApp.exe across DeviceNetworkEvents. Created by Dan/mr-r3b00t/@UK_Daniel_Card

`domains.txt` - Contains list of domains seen as IOCs published by SentinelOne

`hashes.txt` - Contains list of hashes SentinelOne

## Samples

Disclaimer: **VX-UNDERGROUND SAMPLE LINK CONTAINS MALWARE BROWSE AT YOUR OWN RISK**

Windows sample analysis:

https://news.sophos.com/en-us/2023/03/29/3cx-dll-sideloading-attack/

Direct Windows samples:
- ```https://share.vx-underground.org/SmoothOperator.7z```


MacOS sample analysis:

https://twitter.com/patrickwardle/status/1641294247877021696

## Detection content

- Yara: https://github.com/Neo23x0/signature-base/blob/master/yara/gen_mal_3cx_compromise_mar23.yar

- Sigma: https://github.com/SigmaHQ/sigma/pull/4151/files

## Thanks to

- Dan/mr-r3b00t/[@UK_Daniel_Card](https://twitter.com/UK_Daniel_Card) for putting these together in the first place.
- [Sam0x90](https://twitter.com/Sam0x90) for compiling a list of resources.
