# ChallengeProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | Search | [ChallengeProtocol::Search_V1](#challengeprotocolsearch_v1) |
| 2 | Join | [ChallengeProtocol::Join_V1](#challengeprotocoljoin_v1) |
| 3 | WriteProgression | [ChallengeProtocol::WriteProgression_V1](#challengeprotocolwriteprogression_v1) |
| 4 | ReadProgressions | [ChallengeProtocol::ReadProgressions_V1](#challengeprotocolreadprogressions_v1) |

# (1) Search

## ChallengeProtocol::Search_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [ChallengeList](#challengelist-structure) | challenges |

# (2) Join

## ChallengeProtocol::Join_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (3) WriteProgression

## ChallengeProtocol::WriteProgression_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [ChallengeProgression](#challengeprogression-structure) | progression |

# (4) ReadProgressions

## ChallengeProtocol::ReadProgressions_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[ChallengeProgression](#challengeprogression-structure)> | progressions |

# Types

## ChallengeList ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist<[ChallengeData](#challengedata-structure)> | data |
| uint32 | unkUint |

## ChallengeData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| string | unkStr |
| uint32 | unkUint2 |
| uint64 | unkLong1 |
| uint64 | unkLong2 |
| uint64 | unkLong3 |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props1 |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props2 |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props3 |
| qlist<[UnkType](#unktype-structure)> | unkObjs |
| bool | unkBool |

## PropertyVariant ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | key |
| variant | value |

## UnkType ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr1 |
| string | unkStr2 |

## ChallengeProgression ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))
Real name unknown.

| Type | Name |
|------|------|
| uint32 | unkUint |
| [ChallengeProgressionUnkType1](#challengeprogressionunktype1-structure) | unkObj |
| qlist<[ChallengeProgressionUnkType2](#challengeprogressionunktype2-structure)> | unkObjs2 |
| qlist<[ChallengeProgressionUnkType3](#challengeprogressionunktype3-structure)> | unkObjs2 |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |

## ChallengeProgressionUnkType1 ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |
| uint64 | unkLong |
| uint32 | unkUint |

## ChallengeProgressionUnkType2 ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |
| uint64 | unkLong |
| string | unkStr |
| [ChallengeProgressionUnkType1](#challengeprogressionunktype1-structure) | unkObj |

## ChallengeProgressionUnkType3 ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |
| uint64 | unkLong |
| uint32 | unkUint |

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

