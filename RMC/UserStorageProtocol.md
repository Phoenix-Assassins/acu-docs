# UserStorageProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | SearchContents | [UserStorageProtocol::SearchContents_V1](#userstorageprotocolsearchcontents_v1) |
| 2 | SearchContentsWithTotal | [UserStorageProtocol::SearchContentsWithTotal_V1](#userstorageprotocolsearchcontentswithtotal_v1) |
| 3 | DeleteContent | [UserStorageProtocol::DeleteContent_V1](#userstorageprotocoldeletecontent_v1) |
| 4 | SaveMetaData | [UserStorageProtocol::SaveMetaData_V1](#userstorageprotocolsavemetadata_v1) |
| 5 | SaveContentDB | [UserStorageProtocol::SaveContentDB_V1](#userstorageprotocolsavecontentdb_v1) |
| 6 | SaveContentAndGetUploadInfo | [UserStorageProtocol::SaveContentAndGetUploadInfo_V1](#userstorageprotocolsavecontentandgetuploadinfo_v1) |
| 7 | UploadEnd | [UserStorageProtocol::UploadEnd_V1](#userstorageprotocoluploadend_v1) |
| 8 | UpdateExternalContent | [UserStorageProtocol::UpdateExternalContent_V1](#userstorageprotocolupdateexternalcontent_v1) |
| 9 | GetContentDB | [UserStorageProtocol::GetContentDB_V1](#userstorageprotocolgetcontentdb_v1) |
| 10 | GetContentURL | [UserStorageProtocol::GetContentURL_V1](#userstorageprotocolgetcontenturl_v1) |
| 11 | GetContentURLAndSize | [UserStorageProtocol::GetContentURLAndSize_V1](#userstorageprotocolgetcontenturlandsize_v1) |
| 12 | GetMetaData | [UserStorageProtocol::GetMetaData_V1](#userstorageprotocolgetmetadata_v1) |
| 13 | Like | [UserStorageProtocol::Like_V1](#userstorageprotocollike_v1) |
| 14 | Dislike | [UserStorageProtocol::Dislike_V1](#userstorageprotocoldislike_v1) |
| 15 | ResetLikeState | [UserStorageProtocol::ResetLikeState_V1](#userstorageprotocolresetlikestate_v1) |
| 16 | GetLikeState | [UserStorageProtocol::GetLikeState_V1](#userstorageprotocolgetlikestate_v1) |
| 17 | GetFavorites | [UserStorageProtocol::GetFavorites_V1](#userstorageprotocolgetfavorites_v1) |
| 18 | MakeFavorite | [UserStorageProtocol::MakeFavorite_V1](#userstorageprotocolmakefavorite_v1) |
| 19 | RemoveFromFavorites | [UserStorageProtocol::RemoveFromFavorites_V1](#userstorageprotocolremovefromfavorites_v1) |
| 20 | ReportInappropriate | [UserStorageProtocol::ReportInappropriate_V1](#userstorageprotocolreportinappropriate_v1) |
| 21 | IncrementPlayCount | [UserStorageProtocol::IncrementPlayCount_V1](#userstorageprotocolincrementplaycount_v1) |
| 22 | UpdateCustomStat | [UserStorageProtocol::UpdateCustomStat_V1](#userstorageprotocolupdatecustomstat_v1) |
| 23 | GetOwnContents | [UserStorageProtocol::GetOwnContents_V1](#userstorageprotocolgetowncontents_v1) |
| 24 | GetMostPopularTags | [UserStorageProtocol::GetMostPopularTags_V1](#userstorageprotocolgetmostpopulartags_v1) |
| 25 | GetTags | [UserStorageProtocol::GetTags_V1](#userstorageprotocolgettags_v1) |
| 26 | TagContent | [UserStorageProtocol::TagContent_V1](#userstorageprotocoltagcontent_v1) |
| 27 | SearchContentsByPlayers | [UserStorageProtocol::SearchContentsByPlayers_V1](#userstorageprotocolsearchcontentsbyplayers_v1) |
| 28 | SearchContentsByPlayersWithTotal | [UserStorageProtocol::SearchContentsByPlayersWithTotal_V1](#userstorageprotocolsearchcontentsbyplayerswithtotal_v1) |
| 29 | Rate | [UserStorageProtocol::Rate_V1](#userstorageprotocolrate_v1) |
| 30 | GetStarRating | [UserStorageProtocol::GetStarRating_V2](#userstorageprotocolgetstarrating_v2) |
| 31 | GetRemainingQuota | [UserStorageProtocol::GetRemainingQuota_V1](#userstorageprotocolgetremainingquota_v1) |
| 32 | GetTotalQuota | [UserStorageProtocol::GetTotalQuota_V1](#userstorageprotocolgettotalquota_v1) |
| 33 | GetFeed | [UserStorageProtocol::GetFeed_V1](#userstorageprotocolgetfeed_v1) |

# (1) SearchContents

## UserStorageProtocol::SearchContents_V1

### Request

| Type | Name |
|------|------|
| [UserStorageQuery](#userstoragequery-structure) | query |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |

# (2) SearchContentsWithTotal

## UserStorageProtocol::SearchContentsWithTotal_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |
| uint32 | unkUint |

# (3) DeleteContent

## UserStorageProtocol::DeleteContent_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (4) SaveMetaData

## UserStorageProtocol::SaveMetaData_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |

# (5) SaveContentDB

## UserStorageProtocol::SaveContentDB_V1

### Request

| Type | Name |
|------|------|
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | props |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | content |
| [UserContentKey](#usercontentkey-structure) | key |

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |

# (6) SaveContentAndGetUploadInfo

## UserStorageProtocol::SaveContentAndGetUploadInfo_V1

### Request

| Type | Name |
|------|------|
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | props |
| [UserContentKey](#usercontentkey-structure) | key |
| qlist<[ContentUploadRequest](#contentuploadrequest-structure)> | request |

### Response

| Type | Name |
|------|------|
| qlist<[ContentUploadResponse](#contentuploadresponse-structure)> | responses |
| uint64 | unkLong |

# (7) UploadEnd

## UserStorageProtocol::UploadEnd_V1

### Request

| Type | Name |
|------|------|
| uint64 | unkLong |
| [UserContentKey](#usercontentkey-structure) | key |

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |

# (8) UpdateExternalContent

## UserStorageProtocol::UpdateExternalContent_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[ContentUploadResponse](#contentuploadresponse-structure)> | responses |

# (9) GetContentDB

## UserStorageProtocol::GetContentDB_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |

### Response

| Type | Name |
|------|------|
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | content |

# (10) GetContentURL

## UserStorageProtocol::GetContentURL_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<string> | urls |

# (11) GetContentURLAndSize

## UserStorageProtocol::GetContentURLAndSize_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |

### Response

| Type | Name |
|------|------|
| qlist<string> | urls |
| qlist\<uint> | sizes |

# (12) GetMetaData

## UserStorageProtocol::GetMetaData_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |
| [profileid](#profileid-structure) | pid |
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | props |

# (13) Like

## UserStorageProtocol::Like_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (14) Dislike

## UserStorageProtocol::Dislike_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (15) ResetLikeState

## UserStorageProtocol::ResetLikeState_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (16) GetLikeState

## UserStorageProtocol::GetLikeState_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | state |

# (17) GetFavorites

## UserStorageProtocol::GetFavorites_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |
| uint32 | unkUint |

# (18) MakeFavorite

## UserStorageProtocol::MakeFavorite_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (19) RemoveFromFavorites

## UserStorageProtocol::RemoveFromFavorites_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (20) ReportInappropriate

## UserStorageProtocol::ReportInappropriate_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (21) IncrementPlayCount

## UserStorageProtocol::IncrementPlayCount_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (22) UpdateCustomStat

## UserStorageProtocol::UpdateCustomStat_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (23) GetOwnContents

## UserStorageProtocol::GetOwnContents_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |

# (24) GetMostPopularTags

## UserStorageProtocol::GetMostPopularTags_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[Tag](#tag-structure)> | tags |
| uint32 | unkUint |

# (25) GetTags

## UserStorageProtocol::GetTags_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist\<uint32> | tags |

# (26) TagContent

## UserStorageProtocol::TagContent_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (27) SearchContentsByPlayers

## UserStorageProtocol::SearchContentsByPlayers_V1

### Request

| Type | Name |
|------|------|
| qlist<[profileid](#profileid-structure)> | pids |
| [UserStorageQuery](#userstoragequery-structure) | query |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |

# (28) SearchContentsByPlayersWithTotal

## UserStorageProtocol::SearchContentsByPlayersWithTotal_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |
| uint32 | unkUint |

# (29) Rate

## UserStorageProtocol::Rate_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (30) GetStarRating

## UserStorageProtocol::GetStarRating_V2

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| uint32 | unkUint3 |

# (31) GetRemainingQuota

## UserStorageProtocol::GetRemainingQuota_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | count |

# (32) GetTotalQuota

## UserStorageProtocol::GetTotalQuota_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | count |

# (33) GetFeed

## UserStorageProtocol::GetFeed_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | contents |
| uint32 | unkUint |

# Types

## UserStorageQuery ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| [ResultRange](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#resultrange-structure) | range |
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | props |

## PropertyVariant2 ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| variant | variant |

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

## UserContent ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | key |
| [profileid](#profileid-structure) | pid |
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | props |

## UserContentKey ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| uint64 | unkLong |

## ContentUploadRequest ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

## ContentUploadResponse ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr |
| qlist<string> | unkStrings |

## Tag ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
