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
The `onChatMessageCreatedEvent` event is called when a new chat message has been created within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the chat message originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the created message entity from the event.
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
The `onChatMessageDeletedEvent` event is called when a chat message has been deleted within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the chat message originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the deleted message entity from the event.
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
The `onChatMessageUpdateEvent` event is called when a chat message has been updated within Guilded.
### Functions <!-- {docsify-ignore} -->
#### getJGAPI() <!-- {docsify-ignore} -->
Returns the instance of JG_API that is currently being used.
#### getServerId() <!-- {docsify-ignore} -->
Returns the string id of the server the chat message originated from.
#### getMessage() <!-- {docsify-ignore} -->
Returns the updated message entity from the event.
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
## onDocDeletedEvent
## onDocUpdatedEvent

## onListItemCompletedEvent
## onListItemCreatedEvent
## onListItemDeletedEvent
## onListItemUncompletedEvent
## onListItemUpdatedEvent

## onTeamChannelCreatedEvent
## onTeamChannelDeletedEvent
## onTeamChannelUpdatedEvent

## onTeamMemberBannedEvent
## onTeamMemberJoinedEvent
## onTeamMemberRemovedEvent
## onTeamMemberUnbannedEvent
## onTeamMemberUpdatedEvent
## onTeamRolesUpdatedEvent

## onTeamWebhookCreatedEvent
## onTeamWebhookUpdatedEvent