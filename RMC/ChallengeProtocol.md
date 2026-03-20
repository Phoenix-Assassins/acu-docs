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

| Type | Name |
|------|------|
| [ChallengeSearchQuery](#challengesearchquery-structure) | query |

### Response

| Type | Name |
|------|------|
| [ChallengeSearchResult](#challengesearchresult-structure) | result |

# (2) Join

## ChallengeProtocol::Join_V1

### Request

| Type | Name |
|------|------|
| [ChallengeJoinData](#challengejoindata-structure) | joinData |

### Response

This method does not return anything.

# (3) WriteProgression

## ChallengeProtocol::WriteProgression_V1

### Request

| Type | Name |
|------|------|
| [ChallengeProgressionUpdate](#challengeprogressionupdate-structure) | challengeProgressionUpdate |

### Response

| Type | Name |
|------|------|
| [ChallengeProgression](#challengeprogression-structure) | challengeProgression |

# (4) ReadProgressions

## ChallengeProtocol::ReadProgressions_V1

### Request

| Type | Name |
|------|------|
| [ChallengeProgressionQuery](#challengeprogressionquery-structure) | query |

### Response

| Type | Name |
|------|------|
| qlist<[ChallengeProgression](#challengeprogression-structure)> | results |

# Types

## ChallengeSearchQuery ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist\<uint32> | m_availabilities |
| qlist\<string> | m_categories |
| uint32 | m_joinStatus |
| ResultRange | m_range |

## ChallengeSearchResult ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist<[ChallengeDefinition](#challengedefinition-structure)> | m_challengeDefinitions |
| uint32 | m_totalResultCount |

## ChallengeDefinition ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_challengeId |
| string | m_category |
| uint32 | m_availability |
| datetime | m_startTeaseTime |
| datetime | m_startAvailabilityTime |
| datetime | m_endAvailabilityTime |
| std_map\<string,variant> | m_joinParams |
| std_map\<string,variant> | m_progressionParams |
| std_map\<string,variant> | m_extraParams |
| std_map\<string,string> | m_localizedStrings |
| bool | m_hasJoined |

## ChallengeJoinData ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_challengeId |
| std_map\<string,variant> | m_joinParams |

## ChallengeProgressionUpdate ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_challengeId |
| std_map\<string,variant> | m_progressionParams |

## ChallengeProgression ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_challengeId |
| [Progression](#progression-structure) | m_globalProgression |
| std_map<[profileid](#profileid-structure),[PlayerProgression](#playerprogression-structure)> | m_playerProgressions |
| std_map<string,[Progression](#progression-structure)> | m_teamProgressions |
| std_map<string,variant> | m_returnValues |

## Progression ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| std_map\<string,variant> | m_parameters |
| datetime | m_lastUpdate |
| uint32 | m_state |

## PlayerProgression ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| datetime | m_joinTime |
| string | m_team |
| [Progression](#progression-structure) | m_progression |

## ChallengeProgressionQuery ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist<[ProgressionQueryElement](#progressionqueryelement-structure)> | m_queryElements |
| qlist<[profileid](#profileid-structure)> | m_pids |

## ProgressionQueryElement ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_challengeId |
| qlist\<string> | m_teams |

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
