# onChatMessageUpdatedEvent
## Description
The `onChatMessageUpdateEvent` event is called when a chat message has been updated within Guilded.
## Functions
### getJGAPI()
Returns the instance of JG_API that is currently being used.
### getServerId()
Returns the string id of the server the chat message originated from.
### getMessage()
Returns the updated message entity from the event.
## Example Usage
 ```
 @Override
 public void onChatMessageUpdatedEvent(ChatMessageUpdatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ChatMessage message = event.getMessage();
 }
 ```
 ## Last Updated
 2022/06/15