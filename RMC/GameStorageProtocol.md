# GameStorageProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | GetGameParamaters | [GameStorageProtocol::GetGameParamaters_V1](#gamestorageprotocolgetgameparameters_v1) |

# (1) GetGameParamaters

## GameStorageProtocol::GetGameParamaters_V1

### Request

| Type | Name |
|------|------|
| qlist<string> | unkStrings |

### Response

| Type | Name |
|------|------|
| qlist<[GroupInfo](#groupinfo-structure)> | groupInfos |
| qlist<[GameParameters](#gameparameters-structure)> | gameParams |

# Types

## GroupInfo ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr |
| uint32 | unkUint |

## GameParameters ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | unkStr1 |
| string | unkStr2 |
| [Buffer](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#buffer) | data |
