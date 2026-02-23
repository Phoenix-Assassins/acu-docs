# FriendSyncProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | SyncFriends | [FriendSyncProtocol::SyncFriends_V1](#friendsyncprotocolsyncfriends_v1) |

# (1) SyncFriends

## FriendSyncProtocol::SyncFriends_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[profileid]> | pids |

### Response

| Type | Name |
|------|------|
| qlist<[profileid]> | pids |

# Types

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
