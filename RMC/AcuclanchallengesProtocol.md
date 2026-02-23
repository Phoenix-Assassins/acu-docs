# AcuclanchallengesProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | ReportScore | [AcuclanchallengesProtocol::ReportScore_V1](#acuclanchallengesprotocolreportscore_v1) |
| 2 | GetChallengeDetails | [AcuclanchallengesProtocol::GetChallengeDetails_V1](#acuclanchallengesprotocolgetchallengedetails_v1) |
| 3 | GetPoolDetails | [AcuclanchallengesProtocol::GetPoolDetails_v1](#acuclanchallengesprotocolgetpooldetails_v1) |
| 4 | ExportEnums | [AcuclanchallengesProtocol::ExportEnums_V1](#acuclanchallengesprotocolexportenums_v1) |

# (1) ReportScore

## AcuclanchallengesProtocol::ReportScore_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| uint32 | unkUint3 |
| uint32 | unkUint4 |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# (2) GetChallengeDetails

## AcuclanchallengesProtocol::GetChallengeDetails_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| [ClanChallenge](#clanchallenge-structure) | challenge |

# (3) GetPoolDetails

## AcuclanchallengesProtocol::GetPoolDetails_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| uint32 | unkUint3 |
| qlist\<uint32> | unkUints1 |
| qlist\<uint32> | unkUints2 |

# (4) ExportEnums

## AcuclanchallengesProtocol::ExportEnums_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | unkUint |

# Types

## ClanChallenge ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| uint64 | unkLong1 |
| uint64 | unkLong2 |
| uint64 | unkLong3 |
| uint64 | unkLong4 |
| uint64 | unkLong5 |
| uint64 | unkLong6 |
| uint64 | unkLong7 |
| uint64 | unkLong8 |
| uint64 | unkLong9 |
| uint64 | unkLong10 |
| uint64 | unkLong11 |
| uint64 | unkLong12 |
