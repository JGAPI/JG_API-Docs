# JG_API Events
---
Explain what they can expect here...

## onReadyEvent
### Description <!-- {docsify-ignore} -->
The `onReadyEvent` event is called when `JG_API` has finished loading and is ready to be used by code accessing it's API.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onReadyEvent(ReadyEvent event) {
    JG_API jg_api = event.getJGAPI();
 }
 ```

## onChatMessageCreatedEvent
### Description <!-- {docsify-ignore} -->
The `onChatMessageCreatedEvent` event is called when a new ChatMessage has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ChatMessage originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the ChatMessage entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onChatMessageCreatedEvent(ChatMessageCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ChatMessage message = event.getMessage();
 }
 ```

## onChatMessageDeletedEvent
### Description <!-- {docsify-ignore} -->
The `onChatMessageDeletedEvent` event is called when a ChatMessage has been deleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ChatMessage originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the deleted ChatMessage entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onChatMessageDeletedEvent(ChatMessageDeletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ChatMessage message = event.getMessage();
 }
 ```

## onChatMessageUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onChatMessageUpdateEvent` event is called when a ChatMessage has been updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ChatMessage originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the updated ChatMessage entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onChatMessageUpdatedEvent(ChatMessageUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ChatMessage message = event.getMessage();
 }
 ```

## onDocCreatedEvent
### Description <!-- {docsify-ignore} -->
The `onDocCreatedEvent` event is called when a Doc has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the Doc originated from.
#### getDoc() <!-- {docsify-ignore} -->
Returns the Doc entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onDocCreatedEvent(DocCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Doc doc = event.getDoc();
 }
 ```
## onDocDeletedEvent
### Description <!-- {docsify-ignore} -->
The `onDocDeletedEvent` event is called when a Doc has been deleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the Doc originated from.
#### getDoc() <!-- {docsify-ignore} -->
Returns the Doc entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onDocDeletedEvent(DocDeletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Doc doc = event.getDoc();
 }
 ```
## onDocUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onDocUpdatedEvent` event is called when a Doc has been updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the Doc originated from.
#### getDoc() <!-- {docsify-ignore} -->
Returns the Doc entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onDocUpdatedEvent(DocUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Doc doc = event.getDoc();
 }
 ```

## onListItemCompletedEvent
### Description <!-- {docsify-ignore} -->
The `onListItemCompletedEvent` event is called when a ListItem has been completed within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ListItem originated from.
#### getListItem() <!-- {docsify-ignore} -->
Returns the ListItem entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onListItemCompletedEvent(ListItemCompletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ListItem listItem = event.getListItem();
 }
 ```
## onListItemCreatedEvent
### Description <!-- {docsify-ignore} -->
The `onListItemCreatedEvent` event is called when a new ListItem has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ListItem originated from.
#### getListItem() <!-- {docsify-ignore} -->
Returns the ListItem entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onListItemCreatedEvent(ListItemCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ListItem listItem = event.getListItem();
 }
 ```
## onListItemDeletedEvent
### Description <!-- {docsify-ignore} -->
The `onListItemDeletedEvent` event is called when a ListItem has been deleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ListItem originated from.
#### getListItem() <!-- {docsify-ignore} -->
Returns the ListItem entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onListItemDeletedEvent(ListItemDeletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ListItem listItem = event.getListItem();
 }
 ```
## onListItemUncompletedEvent
### Description <!-- {docsify-ignore} -->
The `onListItemUncompletedEvent` event is called when a ListItem has been uncompleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ListItem originated from.
#### getListItem() <!-- {docsify-ignore} -->
Returns the ListItem entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onListItemUncompletedEvent(ListItemUncompletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ListItem listItem = event.getListItem();
 }
 ```
## onListItemUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onListItemUpdatedEvent` event is called when a ListItem has been updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ListItem originated from.
#### getListItem() <!-- {docsify-ignore} -->
Returns the ListItem entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onListItemUpdatedEvent(ListItemUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ListItem listItem = event.getListItem();
 }
 ```

## onTeamChannelCreatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamChannelCreatedEvent` event is called when a new TeamChannel has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the TeamChannel originated from.
#### getTeamChannel() <!-- {docsify-ignore} -->
Returns the TeamChannel entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamChannelCreatedEvent(TeamChannelCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    TeamChannel teamChannel = event.getTeamChannel();
 }
 ```
## onTeamChannelDeletedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamChannelDeletedEvent` event is called when a TeamChannel has been deleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the TeamChannel originated from.
#### getTeamChannel() <!-- {docsify-ignore} -->
Returns the TeamChannel entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamChannelDeletedEvent(TeamChannelDeletedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    TeamChannel teamChannel = event.getTeamChannel();
 }
 ```
## onTeamChannelUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamChannelUpdatedEvent` event is called when a TeamChannel has been updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the TeamChannel originated from.
#### getTeamChannel() <!-- {docsify-ignore} -->
Returns the TeamChannel entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamChannelUpdatedEvent(TeamChannelUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    TeamChannel teamChannel = event.getTeamChannel();
 }
 ```

## onTeamMemberBannedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamMemberBannedEvent` event is called when a ServerMemberBan has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ServerMemberBan originated from.
#### getServerMemberBan() <!-- {docsify-ignore} -->
Returns the ServerMemberBan entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamMemberBannedEvent(TeamMemberBannedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ServerMemberBan serverMemberBan = event.getServerMemberBan();
 }
 ```
## onTeamMemberJoinedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamMemberJoinedEvent` event is called when a ServerMember joins within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ServerMember originated from.
#### getServerMember() <!-- {docsify-ignore} -->
Returns the ServerMember entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamMemberJoinedEvent(TeamMemberJoinedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ServerMember serverMember = event.getServerMember();
 }
 ```
## onTeamMemberRemovedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamMemberRemovedEvent` event is called when a ServerMember is removed within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ServerMember originated from.
#### getUserId() <!-- {docsify-ignore} -->
Returns the user ID of the ServerMember who was removed.
#### isKick() <!-- {docsify-ignore} -->
Returns if the member leaving was the result of a kick.
#### isBan() <!-- {docsify-ignore} -->
Returns if the member leaving was the result of a ban.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamMemberRemovedEvent(TeamMemberRemovedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    String userId = event.getUserId();
    boolean isKick = event.isKick();
    boolean isBan = event.isBan();
 }
 ```
## onTeamMemberUnbannedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamMemberUnbannedEvent` event is called when a ServerMemberBan has been revoked within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ServerMemberBan originated from.
#### getServerMemberBan() <!-- {docsify-ignore} -->
Returns the ServerMemberBan entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamMemberUnbannedEvent(TeamMemberUnbannedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ServerMemberBan serverMemberBan = event.getServerMemberBan();
 }
 ```
## onTeamMemberUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamMemberUpdatedEvent` event is called when a ServerMember is updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the ServerMember originated from.
#### getUserInfo() <!-- {docsify-ignore} -->
Returns an object which contains the user ID and nickname of the ServerMember.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamMemberUpdatedEvent(TeamMemberUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Object userInfo = event.getUserInfo();
 }
 ```
## onTeamRolesUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamRolesUpdatedEvent` event is called when a ServerMember has their roles updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the event originated from.
#### getMemberRoleIds() <!-- {docsify-ignore} -->
Returns an object which contains the user ID and role IDs the member currently has after this operation.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamRolesUpdatedEvent(teamRolesUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Object[] memberRoleIds = event.getMemberRoleIds();
 }
 ```

## onTeamWebhookCreatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamWebhookCreatedEvent` event is called when a new webhook is created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the event originated from.
#### getWebhook() <!-- {docsify-ignore} -->
Returns an the Webhook entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamWebhookCreatedEvent(TeamWebhookCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Webhook webhook = event.getWebhook();
 }
 ```
## onTeamWebhookUpdatedEvent
### Description <!-- {docsify-ignore} -->
The `onTeamWebhookCreatedEvent` event is called when a webhook is updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the event originated from.
#### getWebhook() <!-- {docsify-ignore} -->
Returns an the Webhook entity from the event.
### Example Usage <!-- {docsify-ignore} -->
 ```java
 @Override
 public void onTeamWebhookUpdatedEvent(TeamWebhookUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    Webhook webhook = event.getWebhook();
 }
 ```