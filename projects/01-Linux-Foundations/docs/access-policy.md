# Northstar Access Policy

## Groups
+ developers
+ operations
+ security
+ platform-eng

## users and their groups
| User | Group |
| :----: | :-----: |
| johndev | developers |
| janedev | developers |
| marydev | developers |
| johnengr | platform-eng |
| janeengr | platform-eng |
| maryengr | platform-eng |
| johnsecurity | security |
| janesecurity | security |
| marysecurity | security |
| johnoperations | operations |
| janeoperations | operations |
| maryoperations | operations |

## Access rules
| Group | Folder | permission |
| :----:| :----: |  :----: |
| developers | development | rwxrws--- |
| platform-eng | platform-engineering | rwxrws--- |
| operations | operations | rwxrws--- |
| security | security-&-compliance | rwxrws--- |

## Shared folder
All department folders were created under a shared folder: /srv/northstar. All members have access to this shared folder but within the shared folder, they only have access to their respective departments' folders