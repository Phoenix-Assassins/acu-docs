# PlayerStats2Protocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | PostEvent | [PlayerStats2Protocol::PostEvent_V1](#playerstats2protocolpostevent_v1) |
| 2 | PostEvents | [PlayerStats2Protocol::PostEvents_V1](#playerstats2protocolpostevents_v1) |
| 3 | GetStatistics | [PlayerStats2Protocol::GetStatistics_V1](#playerstats2protocolgetstatistics_v1) |
| 4 | GetStatisticsForPlayers | [PlayerStats2Protocol::GetStatisticsForPlayers_V1](#playerstats2protocolgetstatisticsforplayers_v1) |
| 5 | GetStatisticGroup | [PlayerStats2Protocol::GetStatisticGroup_V1](#playerstats2protocolgetstatisticgroup_v1) |
| 6 | GetStatisticGroupForPlayers | [PlayerStats2Protocol::GetStatisticGroupForPlayers_V1](#playerstats2protocolgetstatisticgroupforplayers_v1) |
| 7 | GetStatisticsForPopulations | [PlayerStats2Protocol::GetStatisticsForPopulations_V1](#playerstats2protocolgetstatisticsforpopulations_v1) |
| 8 | GetLeaderboard | [PlayerStats2Protocol::GetLeaderboard_V1](#playerstats2protocolgetleaderboard_v1) |
| 9 | GetLeaderboardForPlayers | [PlayerStats2Protocol::GetLeaderboardForPlayers_V1](#playerstats2protocolgetleaderboardforplayers_v1) |
| 10 | GetLeaderboardNearPlayer | [PlayerStats2Protocol::GetLeaderboardNearPlayer_V1](#playerstats2protocolgetleaderboardnearplayer_v1) |
| 11 | GetLeaderboardCenteredOnPlayer | [PlayerStats2Protocol::GetLeaderboardCenteredOnPlayer_V1](#playerstats2protocolgetleaderboardcenteredonplayer_v1) |
| 12 | GetLeaderboardForPopulations | [PlayerStats2Protocol::GetLeaderboardForPopulations_V1](#playerstats2protocolgetleaderboardforpopulations_v1) |
| 13 | GetLeaderboardNearPopulation | [PlayerStats2Protocol::GetLeaderboardNearPopulation_V1](#playerstats2protocolgetleaderboardnearpopulation_v1) |
| 14 | GetLeaderboardCenteredOnPopulation | [PlayerStats2Protocol::GetLeaderboardCenteredOnPopulation_V1](#playerstats2protocolgetleaderboardcenteredonpopulation_v1) |

# (1) PostEvent

## PlayerStats2Protocol::PostEvent_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (2) PostEvents

## PlayerStats2Protocol::PostEvents_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (3) GetStatistics

## PlayerStats2Protocol::GetStatistics_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [PlayerStatistics](#playerstatistics-structure) | stats |

# (4) GetStatisticsForPlayers

## PlayerStats2Protocol::GetStatisticsForPlayers_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[PlayerStatistics](#playerstatistics-structure)> | stats |

# (5) GetStatisticGroup

## PlayerStats2Protocol::GetStatisticGroup_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [PlayerStatistics](#playerstatistics-structure) | stats |

# (6) GetStatisticGroupForPlayers

## PlayerStats2Protocol::GetStatisticGroupForPlayers_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[PlayerStatistics](#playerstatistics-structure)> | stats |

# (7) GetStatisticsForPopulations

## PlayerStats2Protocol::GetStatisticsForPopulations_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[PlayerStatistics](#playerstatistics-structure)> | stats |

# (8) GetLeaderboard

## PlayerStats2Protocol::GetLeaderboard_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (9) GetLeaderboardForPlayers

## PlayerStats2Protocol::GetLeaderboardForPlayers_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (10) GetLeaderboardNearPlayer

## PlayerStats2Protocol::GetLeaderboardNearPlayer_V1

### Request

| Type | Name |
|------|------|
| string | unkStr |
| uint32 | unkUint |

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (11) GetLeaderboardCenteredOnPlayer

## PlayerStats2Protocol::GetLeaderboardCenteredOnPlayer_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (12) GetLeaderboardForPopulations

## PlayerStats2Protocol::GetLeaderboardForPopulations_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (13) GetLeaderboardNearPopulation

## PlayerStats2Protocol::GetLeaderboardNearPopulation_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# (14) GetLeaderboardCenteredOnPopulation

## PlayerStats2Protocol::GetLeaderboardCenteredOnPopulation_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [Leaderboard](#leaderboard-structure) | leaderboard |

# Types

## PropertyVariant ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | key |
| variant | value |

## PlayerStatistics ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr |
| qlist<[PropertyVariant](#propertyvariant-structure)> | stats |

## Leaderboard ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[LeaderboardRow](#leaderboardrow-structure)> | rows |

## LeaderboardRow ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr |
| uint32 | unkUint |
| uint64 | unkLong |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |
