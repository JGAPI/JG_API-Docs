# onChatMessageCreatedEvent
## Description
The `onChatMessageCreatedEvent` event is called when a new chat message has been created within Guilded.
## Functions
### getJGAPI()
Returns the instance of JG_API that is currently being used.
### getServerId()
Returns the string id of the server the chat message originated from.
### getMessage()
Returns the created message entity from the event.
## Example Usage
 ```java
 @Override
 public void onChatMessageCreatedEvent(ChatMessageCreatedEvent event) {
    JG_API jg_api = event.getJGAPI();
    String serverId = event.getServerId();
    ChatMessage message = event.getMessage();
 }
 ```
 ## Last Updated
 2022/06/15