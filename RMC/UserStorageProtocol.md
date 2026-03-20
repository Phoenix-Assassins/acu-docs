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
| qlist<[UserContent](#usercontent-structure)> | searchResults |

# (2) SearchContentsWithTotal

## UserStorageProtocol::SearchContentsWithTotal_V1

### Request

| Type | Name |
|------|------|
| [UserStorageQuery](#userstoragequery-structure) | query |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | searchResults |
| uint32 | totalResults |

# (3) DeleteContent

## UserStorageProtocol::DeleteContent_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (4) SaveMetaData

## UserStorageProtocol::SaveMetaData_V1

### Request

| Type | Name |
|------|------|
| qlist<PropertyVariant> | properties |
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

# (5) SaveContentDB

## UserStorageProtocol::SaveContentDB_V1

### Request

| Type | Name |
|------|------|
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | properties |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | data |
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

# (6) SaveContentAndGetUploadInfo

## UserStorageProtocol::SaveContentAndGetUploadInfo_V1

### Request

| Type | Name |
|------|------|
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | properties |
| [UserContentKey](#usercontentkey-structure) | contentKey |
| qlist<[ContentUploadRequest](#contentuploadrequest-structure)> | uploadRequests |

### Response

| Type | Name |
|------|------|
| qlist<[ContentUploadResponse](#contentuploadresponse-structure)> | uploadResponses |
| uint64 | pendingID |

# (7) UploadEnd

## UserStorageProtocol::UploadEnd_V1

### Request

| Type | Name |
|------|------|
| uint64 | pendingID |
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

# (8) UpdateExternalContent

## UserStorageProtocol::UpdateExternalContent_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |
| qlist<[ContentUploadRequest](#contentuploadrequest-structure)> | uploadRequests |

### Response

| Type | Name |
|------|------|
| qlist<[ContentUploadResponse](#contentuploadresponse-structure)> | uploadResponses |

# (9) GetContentDB

## UserStorageProtocol::GetContentDB_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | data |

# (10) GetContentURL

## UserStorageProtocol::GetContentURL_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| qlist\<string> | downloadURLs |

# (11) GetContentURLAndSize

## UserStorageProtocol::GetContentURLAndSize_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| qlist\<string> | downloadURLs |
| qlist\<uint32> | size |

# (12) GetMetaData

## UserStorageProtocol::GetMetaData_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| [UserContent](#usercontent-structure) | content |

# (13) Like

## UserStorageProtocol::Like_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (14) Dislike

## UserStorageProtocol::Dislike_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (15) ResetLikeState

## UserStorageProtocol::ResetLikeState_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (16) GetLikeState

## UserStorageProtocol::GetLikeState_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| int32 | state |

# (17) GetFavorites

## UserStorageProtocol::GetFavorites_V1

### Request

| Type | Name |
|------|------|
| uint32 | contentType |
| uint32 | offset |
| uint32 | count |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | favorites |
| uint32 | total |

# (18) MakeFavorite

## UserStorageProtocol::MakeFavorite_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (19) RemoveFromFavorites

## UserStorageProtocol::RemoveFromFavorites_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (20) ReportInappropriate

## UserStorageProtocol::ReportInappropriate_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |
| string | reason |

### Response

This method does not return anything.

# (21) IncrementPlayCount

## UserStorageProtocol::IncrementPlayCount_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

This method does not return anything.

# (22) UpdateCustomStat

## UserStorageProtocol::UpdateCustomStat_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |
| uint16 | statID |
| int64 | incValue |

### Response

This method does not return anything.

# (23) GetOwnContents

## UserStorageProtocol::GetOwnContents_V1

### Request

| Type | Name |
|------|------|
| uint32 | typeID |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | results |

# (24) GetMostPopularTags

## UserStorageProtocol::GetMostPopularTags_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| qlist<[WeightedTag](#weightedtag-structure)> | tags |
| uint32 | totalNumberOfTaggings |

# (25) GetTags

## UserStorageProtocol::GetTags_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| qlist\<uint32> | tagIds |

# (26) TagContent

## UserStorageProtocol::TagContent_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |
| qlist\<uint32> | newTagIds |

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
| qlist<[UserContent](#usercontent-structure)> | searchResults |

# (28) SearchContentsByPlayersWithTotal

## UserStorageProtocol::SearchContentsByPlayersWithTotal_V1

### Request

| Type | Name |
|------|------|
| qlist<[profileid](#profileid-structure)> | pids |
| [UserStorageQuery](#userstoragequery-structure) | query |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | searchResults |
| uint32 | totalResults |

# (29) Rate

## UserStorageProtocol::Rate_V1

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |
| uint32 | rating |

### Response

This method does not return anything.

# (30) GetStarRating

## UserStorageProtocol::GetStarRating_V2

### Request

| Type | Name |
|------|------|
| [UserContentKey](#usercontentkey-structure) | contentKey |

### Response

| Type | Name |
|------|------|
| uint32 | rating |
| uint32 | totalRatings |
| float | averageRating |

# (31) GetRemainingQuota

## UserStorageProtocol::GetRemainingQuota_V1

### Request

| Type | Name |
|------|------|
| uint32 | typeID |

### Response

| Type | Name |
|------|------|
| uint32 | remainingQuota |

# (32) GetTotalQuota

## UserStorageProtocol::GetTotalQuota_V1

### Request

| Type | Name |
|------|------|
| uint32 | typeID |

### Response

| Type | Name |
|------|------|
| uint32 | totalQuota |

# (33) GetFeed

## UserStorageProtocol::GetFeed_V1

### Request

| Type | Name |
|------|------|
| string | name |
| ResultRange | resultRange |

### Response

| Type | Name |
|------|------|
| qlist<[UserContent](#usercontent-structure)> | feedResults |
| uint32 | totalResults |

# Types

## UserStorageQuery ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_typeID |
| uint32 | m_queryID |
| [ResultRange](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#resultrange-structure) | m_resultRange |
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | m_parameters |

## PropertyVariant2 ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_ID |
| variant | m_value |

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
| [UserContentKey](#usercontentkey-structure) | m_key |
| [profileid](#profileid-structure) | m_pid |
| qlist<[PropertyVariant2](#propertyvariant2-structure)> | m_properties |

## UserContentKey ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_typeID |
| uint64 | m_contentID |

## ContentUploadRequest ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_mimeTypeID |
| uint32 | m_size |

## ContentUploadResponse ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | m_contentUrl |
| qlist\<string> | m_headers |

## WeightedTag ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | m_id |
| uint32 | m_numberOfOccurences |
