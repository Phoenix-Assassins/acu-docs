# MatchmakingProtocol

| ID | Method | Variant |
|----|--------|---------|
| 1 | CreateMatchTicket | [MatchmakingProtocol::CreateMatchTicket_V1](#matchmakingprotocolcreatematchticket_v1) |
| 2 | CreatePushTicket | [MatchmakingProtocol::CreatePushTicket_V1](#matchmakingprotocolcreatepushticket_v1) |
| 3 | UpdateTicket | [MatchmakingProtocol::UpdateTicket_V1](#matchmakingprotocolupdateticket_v1) |
| 4 | CancelTicket | [MatchmakingProtocol::CancelTicket_V1](#matchmakingprotocolcancelticket_v1) |
| 5 | CancelAllTicket | [MatchmakingProtocol::CancelAllTicket_V1](#matchmakingprotocolcancelallticket_v1) |
| 6 | CreateSession | [MatchmakingProtocol::CreateSession_V1](#matchmakingprotocolcreatesession_v1) |
| 7 | ReserveSessionId | [MatchmakingProtocol::ReserveSessionId_V1](#matchmakingprotocolreservesessionid_v1) |
| 8 | CreateSessionWithReservedId | [MatchmakingProtocol::CreateSessionWithReservedId_V1](#matchmakingprotocolcreatesessionwithreservedid_v1) |
| 9 | UpdateSession | [MatchmakingProtocol::UpdateSession_V1](#matchmakingprotocolupdatesession_v1) |
| 10 | LeaveSession | [MatchmakingProtocol::LeaveSession_V1](#matchmakingprotocolleavesession_v1) |
| 11 | GetSession | [MatchmakingProtocol::GetSession_V1](#matchmakingprotocolgetsession_v1) |
| 12 | GetMemberSessions | [MatchmakingProtocol::GetMemberSessions_V2](#matchmakingprotocolgetmembersessions_v2) |
| 13 | MigrateHost | [MatchmakingProtocol::MigrateHost_V1](#matchmakingprotocolmigratehost_v1) |
| 14 | JoinSession | [MatchmakingProtocol::JoinSession_V1](#matchmakingprotocoljoinsession_v1) |
| 15 | JoinPlayer | [MatchmakingProtocol::JoinPlayer_V1](#matchmakingprotocoljoinplayer_v1) |
| 16 | AddMembers | [MatchmakingProtocol::AddMembers_V1](#matchmakingprotocoladdmembers_v1) |
| 17 | RemoveMembers | [MatchmakingProtocol::RemoveMembers_V1](#matchmakingprotocolremovemembers_v1) |
| 18 | ReportJoinSuccess | [MatchmakingProtocol::ReportJoinSuccess_V1](#matchmakingprotocolreportjoinsuccess_v1) |
| 19 | ReportJoinFailure | [MatchmakingProtocol::ReportJoinFailure_V1](#matchmakingprotocolreportjoinfailure_v1) |
| 20 | SendInvitation | [MatchmakingProtocol::SendInvitation_V1](#matchmakingprotocolsendinvitation_v1) |
| 21 | GetReceivedInvitationsCount | [MatchmakingProtocol::GetReceivedInvitationsCount_V1](#matchmakingprotocolgetreceivedinvitationscount_v1) |
| 22 | GetReceivedInvitations | [MatchmakingProtocol::GetReceivedInvitations_V1](#matchmakingprotocolgetreceivedinvitations_v1) |
| 23 | GetSentInvitationsCount | [MatchmakingProtocol::GetSentInvitationsCount_V1](#matchmakingprotocolgetsentinvitationscount_v1) |
| 24 | GetSentInvitations | [MatchmakingProtocol::GetSentInvitations_V1](#matchmakingprotocolgetsentinvitations_v1) |
| 25 | AcceptInvitation | [MatchmakingProtocol::AcceptInvitation_V1](#matchmakingprotocolacceptinvitation_v1) |
| 26 | DeclineInvitation | [MatchmakingProtocol::DeclineInvitation_V1](#matchmakingprotocoldeclineinvitation_v1) |
| 27 | CancelInvitation | [MatchmakingProtocol::CancelInvitation_V1](#matchmakingprotocolcancelinvitation_v1) |
| 28 | AddPlayerContexts | [MatchmakingProtocol::AddPlayerContexts_V1](#matchmakingprotocoladdplayercontexts_v1) |
| 29 | RemovePlayerContexts | [MatchmakingProtocol::RemovePlayerContexts_V1](#matchmakingprotocolremoveplayercontexts_v1) |

# (1) CreateMatchTicket

## MatchmakingProtocol::CreateMatchTicket_V1

### Request

| Type | Name |
|------|------|
| qlist\<stationurl> | urls |
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| [SearchCriteria](#searchcriteria-structure) | searchCriteria |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

# (2) CreatePushTicket

## MatchmakingProtocol::CreatePushTicket_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| [SearchCriteria](#searchcriteria-structure) | searchCriteria |

### Response

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

# (3) UpdateTicket

## MatchmakingProtocol::UpdateTicket_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist\<[PropertyVariant](#propertyvariant-structure)> | props |

### Response

This method does not return anything.

# (4) CancelTicket

## MatchmakingProtocol::CancelTicket_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (5) CancelAllTicket

## MatchmakingProtocol::CancelAllTicket_V1

### Request

This method does not take any parameters.

### Response

This method does not return anything.

# (6) CreateSession

## MatchmakingProtocol::CreateSession_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | sessionId |

# (7) ReserveSessionId

## MatchmakingProtocol::ReserveSessionId_V1

### Request

This method does not take any parameters.

### Response

| Type | Name |
|------|------|
| uint32 | sessionId |

# (8) CreateSessionWithReservedId

## MatchmakingProtocol::CreateSessionWithReservedId_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |
| qlist\<stationurl> | urls |
| qlist<[SessionMember](#sessionmember-structure)> | members |
| uint32 | unkUint3 |

### Response

| Type | Name |
|------|------|
| uint32 | sessionId |

# (9) UpdateSession

## MatchmakingProtocol::UpdateSession_V1

### Request

| Type | Name |
|------|------|
| uint32 | sessionId |
| qlist\<[PropertyVariant](#propertyvariant-structure)> | props |

### Response

This method does not return anything.

# (10) LeaveSession

## MatchmakingProtocol::LeaveSession_V1

### Request

| Type | Name |
|------|------|
| uint32 | sessionId |

### Response

This method does not return anything.

# (11) GetSession

## MatchmakingProtocol::GetSession_V1

### Request

| Type | Name |
|------|------|
| uint32 | sessionId |

### Response

| Type | Name |
|------|------|
| [MatchmakingSession](#matchmakingsession-structure) | session |

# (12) GetMemberSessions

## MatchmakingProtocol::GetMemberSessions_V2

### Request

| Type | Name |
|------|------|
| qlist<[profileid](#profileid-structure)> | members |

### Response

| Type | Name |
|------|------|
| qlist<[MemberSessions](#membersessions-structure)> | memberSessions |

# (13) MigrateHost

## MatchmakingProtocol::MigrateHost_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist\<stationurl> | urls |

### Response

This method does not return anything.

# (14) JoinSession

## MatchmakingProtocol::JoinSession_V1

### Request

| Type | Name |
|------|------|
| uint32 | sessionId |

### Response

This method does not return anything.

# (15) JoinPlayer

## MatchmakingProtocol::JoinPlayer_V1

### Request

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | joinedPlayer |

### Response

This method does not return anything.

# (16) AddMembers

## MatchmakingProtocol::AddMembers_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (17) RemoveMembers

## MatchmakingProtocol::RemoveMembers_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[profileid](#profileid-structure)> | members |

### Response

This method does not return anything.

# (18) ReportJoinSuccess

## MatchmakingProtocol::ReportJoinSuccess_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint |

### Response

This method does not return anything.

# (19) ReportJoinFailure

## MatchmakingProtocol::ReportJoinFailure_V1

### Request

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |

### Response

This method does not return anything.

# (20) SendInvitation

## MatchmakingProtocol::SendInvitation_V1

### Request

| Type | Name |
|------|------|
| [InvitationRequest](#invitationrequest-structure) | invitation |

### Response

This method does not return anything.

# (21) GetReceivedInvitationsCount

## MatchmakingProtocol::GetReceivedInvitationsCount_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | recvInvitations |

# (22) GetReceivedInvitations

## MatchmakingProtocol::GetReceivedInvitations_V1

### Request

| Type | Name |
|------|------|
| [ResultRange](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#resultrange-structure) | range |

### Response

| Type | Name |
|------|------|
| [ReceivedInvitationsResult](#receivedinvitationsresult-structure) | recvInvResult |

# (23) GetSentInvitationsCount

## MatchmakingProtocol::GetSentInvitationsCount_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| uint32 | sentInvitations |

# (24) GetSentInvitations

## MatchmakingProtocol::GetSentInvitations_V1

### Request

Unused method, payload unknown.

### Response

| Type | Name |
|------|------|
| [ReceivedInvitationsResult](#receivedinvitationsresult-structure) | sentInvResult |

# (25) AcceptInvitation

## MatchmakingProtocol::AcceptInvitation_V1

### Request

| Type | Name |
|------|------|
| [Invitation](#inivitation-structure) | invitation |

### Response

This method does not return anything.

# (26) DeclineInvitation

## MatchmakingProtocol::DeclineInvitation_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (27) CancelInvitation

## MatchmakingProtocol::CancelInvitation_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (28) AddPlayerContexts

## MatchmakingProtocol::AddPlayerContexts_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# (29) RemovePlayerContexts

## MatchmakingProtocol::RemovePlayerContexts_V1

### Request

Unused method, payload unknown.

### Response

This method does not return anything.

# Types

## SearchCriteria ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist\<[PropertyVariant](#propertyvariant-structure)> | props |
| qlist\<uint32> | unkUints |
| uint16 | unkUint |

## PropertyVariant ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| string | key |
| variant | value |

## SessionMember ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | pid |
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

## MatchmakingSession ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint1 |
| uint32 | unkUint2 |
| datetime | time |
| qlist<[PropertyVariant](#propertyvariant-structure)> | props |
| [SessionMember](#sessionmember-structure) | host |
| qlist\<string> | unkStrings |
| qlist<[SessionMember](#sessionmember-structure)> | members |
| uint32 | unkUint3 |
| uint32 | unkUint4 |
| bool | unkBool |

## MemberSessions ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| [profileid](#profileid-structure) | memberPid |
| qlist<[MatchmakingSession](#matchmakingsession-structure)> | sessions |

## InvitationRequest ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | unkUint |
| qlist<[profileid](#profileid-structure)> | members |
| string | unkStr |

## Inivitation ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| uint32 | sessionId |
| [profileid](#profileid-structure) | pid |
| string | unkStr |
| datetime | time |

## ReceivedInvitationsResult ([Structure](https://github.com/kinnay/NintendoClients/wiki/NEX-Common-Types#structure))

| Type | Name |
|------|------|
| qlist<[Invitation](#inivitation-structure)> | invitations |
| uint32 | unkUint |