# ChallengeProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | CreateClan | [ClansProtocol::CreateClan_V1](#clansprotocolcreateclan_v1) |
| 2 | RenameClan | [ClansProtocol::RenameClan_V1](#clansprotocolrenameclan_v1) |
| 3 | GetClansInfos | [ClansProtocol::GetClansInfos_V1](#clansprotocolgetclansinfos_v1) |
| 4 | GetClansNames | [ClansProtocol::GetClansNames_V1](#clansprotocolgetclansnames_v1) |
| 5 | GetPlayersClanInfos | [ClansProtocol::GetPlayersClanInfos_V1](#clansprotocolgetplayersclaninfos_v1) |
| 6 | GetMembersLists | [ClansProtocol::GetMembersLists_V1](#clansprotocolgetmemberslists_v1) |
| 7 | InviteToClan | [ClansProtocol::InviteToClan_V1](#clansprotocolinvitetoclan_v1) |
| 8 | AcceptClanInvite | [ClansProtocol::AcceptClanInvite_V1](#clansprotocolacceptclaninvite_v1) |
| 9 | LeaveClan | [ClansProtocol::LeaveClan_V1](#clansprotocolleaveclan_v1) |
| 10 | ChangeRole | [ClansProtocol::ChangeRole_V1](#clansprotocolchangerole_v1) |
| 11 | Kick | [ClansProtocol::Kick_V1](#clansprotocolkick_v1) |
| 12 | WriteClanStats | [ClansProtocol::WriteClanStats_V1](#clansprotocolwriteclanstats_v1) |
| 13 | WriteClanMemberStats | [ClansProtocol::WriteClanMemberStats_V1](#clansprotocolwriteclanmemberstats_v1) |
| 14 | ReadClanStats | [ClansProtocol::ReadClanStats_V1](#clansprotocolreadclanstats_v1) |
| 15 | ReadClanMemberStats | [ClansProtocol::ReadClanMemberStats_V1](#clansprotocolreadclanmemberstats_v1) |
| 16 | SearchClanByStats | [ClansProtocol::SearchClanByStats_V1](#clansprotocolsearchclanbystats_v1) |
| 17 | SearchClanByName | [ClansProtocol::SearchClanByName_V1](#clansprotocolsearchclanbyname_v1) |
| 18 | ApplyToClan | [ClansProtocol::ApplyToClan_V1](#clansprotocolapplytoclan_v1) |
| 19 | GetMyApplication | [ClansProtocol::GetMyApplication_V1](#clansprotocolgetmyapplication_v1) |
| 20 | CancelMyApplication | [ClansProtocol::CancelMyApplication_V1](#clansprotocolcancelmyapplication_v1) |
| 21 | GetClanApplications | [ClansProtocol::GetClanApplications_V1](#clansprotocolgetclanapplications_v1) |
| 22 | AnswerClanApplication | [ClansProtocol::AnswerClanApplication_V1](#clansprotocolanswerclanapplication_v1) |
| 23 | GetClanNotifications | [ClansProtocol::GetClanNotifications_V1](#clansprotocolgetclannotifications_v1) |

# (1) CreateClan

## ClansProtocol::CreateClan_V1

### Request

| Type | Name |
|------|------|
| string | unkStr1 |
| string | unkStr2 |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

# (2) RenameClan

## ClansProtocol::RenameClan_V1

### Request

| Type | Name |
|------|------|
| string | unkStr1 |
| string | unkStr2 |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (3) GetClansInfos

## ClansProtocol::GetClansInfos_V1

### Request

| Type | Name |
|------|------|
| qlist\<uint32> | clanIds |

### Response

| Type | Name |
|------|------|
| qlist<[Clan](#clan-structure)> | clans |

# (4) GetClansNames

## ClansProtocol::GetClansNames_V1

### Request

| Type | Name |
|------|------|
| qlist\<uint32> | clanIds |

### Response

| Type | Name |
|------|------|
| map\<uint32, string> | clanNames |

# (5) GetPlayersClanInfos

## ClansProtocol::GetPlayersClanInfos_V1

### Request

| Type | Name |
|------|------|
| qlist<[profileid](#profileid-structure)> | pids |

### Response

| Type | Name |
|------|------|
| qlist\<uint32> | pids1 |
| qlist\<uint32> | pids2 |

# (6) GetMembersLists

## ClansProtocol::GetMembersLists_V1

### Request

| Type | Name |
|------|------|
| qlist\<uint32> | pids |

### Response

| Type | Name |
|------|------|
| qlist<qlist<[ClanMember](#clanmember-structure)>> | memberLists |

# (7) InviteToClan

## ClansProtocol::InviteToClan_V1

### Request

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (8) AcceptClanInvite

## ClansProtocol::AcceptClanInvite_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (9) LeaveClan

## ClansProtocol::LeaveClan_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (10) ChangeRole

## ClansProtocol::ChangeRole_V1

### Request

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (11) Kick

## ClansProtocol::Kick_V1

### Request

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (12) WriteClanStats

## ClansProtocol::WriteClanStats_V1

### Request

| Type | Name |
|------|------|
| qlist<[ClanStatisticWriteStruct](#clanstatisticwritestruct-structure)> | stats |

### Response

This method does not return anything.

# (13) WriteClanMemberStats

## ClansProtocol::WriteClanMemberStats_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (14) ReadClanStats

## ClansProtocol::ReadClanStats_V1

### Request

| Type | Name |
|------|------|
| qlist<[ClanStatisticData](#clanstatisticdata-structure)> | data |

### Response

| Type | Name |
|------|------|
| qlist<[ClanStatisticListRead](#clanstatisticlistread-structure)> | statLists |

# (15) ReadClanMemberStats

## ClansProtocol::ReadClanMemberStats_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[ClanMemberStatisticReadList](#clanmemberstatisticreadlist-structure)> | statLists |

# (16) SearchClanByStats

## ClansProtocol::SearchClanByStats_V1

### Request

| Type | Name |
|------|------|
| qlist<[ClanStatisticWriteStruct](#clanstatisticwritestruct-structure)> | stats |
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

| Type | Name |
|------|------|
| qlist\<uint32> | clanIds |
| uint32 | unkUint |

# (17) SearchClanByName

## ClansProtocol::SearchClanByName_V1

### Request

| Type | Name |
|------|------|
| string | clanName |
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

| Type | Name |
|------|------|
| qlist\<uint32> | clanIds |
| uint32 | unkUint |

# (18) ApplyToClan

## ClansProtocol::ApplyToClan_V1

### Request

| Type | Name |
|------|------|
| uint32 | clanId |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (19) GetMyApplication

## ClansProtocol::GetMyApplication_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (20) CancelMyApplication

## ClansProtocol::CancelMyApplication_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (21) GetClanApplications

## ClansProtocol::GetClanApplications_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| qlist<[ClanApplication](#clanapplication-structure)> | applications |
| uint32 | unkUint |

# (22) AnswerClanApplication

## ClansProtocol::AnswerClanApplication_V1

### Request

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (23) GetClanNotifications

## ClansProtocol::GetClanNotifications_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| qlist<[ClanNotification](#clannotification-structure)> | notifs |
| uint32 | unkUint |

# Types

## Clan ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| string | unkStr1 |
| string | unkStr2 |
| [profileid](#profileid-structure) | ownerPid |
| uint32 | unkUint2 |
| uint32 | unkUint3 |

## ClanMember ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |
| uint32 | unkUint1 |
| uint32 | unkUint2 |

## profileid ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | pid |
| uint16 | unkShort1 |
| uint16 | unkShort2 |
| uint16 | unkShort3 |
| uint16 | unkShort4 |
| uint16 | unkShort5 |
| uint16 | unkShort6 |

## ClanStatisticWriteStruct ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[ClanStatisticWriteValue](#clanstatisticwritevalue-structure)> | values |

## ClanStatisticWriteValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| bool | unkBool |
| [ClanStatPolicy](#clanstatpolicy-structure) | policy |

## ClanStatPolicy ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| variant | variant |
| uint32 | unkUint |

## ClanStatisticData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<uint8> | unkBytes |

## ClanStatisticListRead ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[ClanStatisticReadStruct](#clanstatisticreadstruct-structure)> | stats |

## ClanStatisticReadStruct ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[ClanStatisticReadValue](#clanstatisticreadvalue-structure)> | values |

## ClanStatisticReadValue ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint8 | key |
| variant | value |

## ClanMemberStatisticReadList ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |
| qlist<[ClanStatisticReadStruct](#clanstatisticreadstruct-structure)> | stats |

## ClanApplication ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| [profileid](#profileid-structure) | pid |
| uint32 | unkUint2 |

## ClanNotification ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| [profileid](#profileid-structure) | pid |
| uint32 | unkUint2 |
| uint32 | unkUint3 |