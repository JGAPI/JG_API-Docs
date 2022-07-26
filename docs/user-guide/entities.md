# JG_API Entities
---
Explain what they can expect here...

## CalendarEvent

### Description
The `CalendarEvent` is the entity returned for events `CalendarEventCreatedEvent`, `CalendarEventDeletedEvent`, `CalendarEventUpdatedEvent`.

### Methods
#### getCalendarId(): Integer
Returns the id of the entity.
#### getServerId(): String
Returns the server id of the entity.
#### getChannelId(): String
Returns the channel id of the entity.
#### getName(): String
Returns the name of the event. Minimum length: `1`; Maximum length: `60`
#### getDescription(): String
Returns the description of the event. Minimum length: `1`; Maximum length: `8000`
#### getLocation(): String
Returns the location of the event. Minimum length: `1`; Maximum length: `8000`
#### getUrl(): String
Returns the URL to associate with the event.
#### getColor(): Integer
Returns the color of the event when viewed in the calendar. Minimum: `0`; Maximum: `16777215`
#### getRsvpLimit(): Integer
Returns the number of RSVPs to allow before waitlisting RSVPs. Minimum: `1`
#### getStartsAt(): Instant
Returns the ISO 8601 timestamp that the event starts at.
#### getDuration(): Integer
Returns the duration of the event in minutes. Minimum: `1`
#### isPrivate(): Boolean
Returns if the CalendarEvent is private or not.
#### getMentions(): Mentions
Returns the Mentions entity of the CalendarEvent entity.
#### getCreatedAt(): Instant
Returns the ISO 8601 timestamp that the event was created at.
#### getCreatedBy(): String
Returns the ID of the user who created this entity.
#### getCancellation(): CalendarEventCancellation
Returns the CalendarEventCancellation entity.

#### setName(String name): RestAction<CalendarEvent>
Creates a RestAction where the name will be set to the specified String `name` parameter.
#### setDescription(String description): RestAction<CalendarEvent>
#### setLocation(String location): RestAction<CalendarEvent>
#### setStart(Instant startsAt): RestAction<CalendarEvent>
#### setUrl(String url): RestAction<CalendarEvent>
#### setColor(int color): RestAction<CalendarEvent>
#### setDuration(int duration): RestAction<CalendarEvent>
#### setPrivate(boolean isPrivate): RestAction<CalendarEvent>
#### delete(): RestAction<CalendarEvent>
#### update(String name, String description, String location, Instant startsAt, String url, int color, int duration, boolean isPrivate): RestAction<CalendarEvent>

## CalendarEventCancellation

### Description
TBD

### Methods
#### getDescription(): String
Returns the description of the event. Minimum length: `1`; Maximum length: `140`
#### getCreatedBy(): String
Returns the ID of the user who created this entity.

## CalenderEventRsvp 

### Description
TBD

### Methods
#### getCalendarEventId(): Integer
Returns the id of the entity.
#### getChannelId(): String
Returns the channel id of the entity.
#### getServerId(): String
Returns the server id of the entity.
#### getUserId(): String
Returns the user id of the entity.
#### getStatus(): String 
Returns the status of the entity.
#### getCreatedBy(): String 
Returns the user id of who created the entity.
#### getCreatedAt(): Instant
Returns the ISO 8601 timestamp that the entity was created at.
#### getUpdatedBy(): String 
Returns the user id of who updated the entity.
#### getUpdatedAt(): Instant
Returns the ISO 8601 timestamp that the entity was updated at.

## ChannelReaction

### Description
TBD

### Methods
#### getChannelId(): String
Returns the channel id of the entity.
#### getMessageId(): String
Returns the message id of the entity.
#### getCreatedBy(): String
Returns the user id of the entity.
#### getEmote(): Emote
Returns the entity Emote used.

## Mentions

### Description
TBD

### Methods
#### getUsers(): String[]
Returns user ids that were mentioned. Minimum Items: `1`
#### getChannels(): String[]
Returns channel ids that were mentioned. Minimum Items: `1`
#### getRoles(): Integer[]
Returns role ids that were mentioned. Minimum Items: `1`
#### isEveryone(): Boolean
Returns a check if @everyone was used.
#### isHere(): Boolean
Returns a check if @here was used.

## ServerChannel

### Description
TBD

### Methods
#### getId(): String
Returns the channel id of the entity.
#### getType(): String
Returns the channel type of the entity.
#### getName(): String
Returns the name of the entity. Minimum length: `1`; Maximum length: `100`
#### getTopic(): String
Returns the topic of the entity. Minimum length: `1`; Maximum length: `512`
#### getCreatedAt(): Instant 
Returns the ISO 8601 timestamp that the entity was created at.
#### getCreatedBy(): String 
Returns the user id of who created the entity.
#### getServerId(): String 
Returns the server id of the entity.
#### getParentId(): String 
Returns the parent id of the entity
#### getCategoryId(): Integer 
Returns the category id of the entity.
#### getGroupId(): String 
Returns the group id of the entity.
#### isPublic(): Boolean 
Returns if the ServerChannel is public or not.
#### getArchivedAt(): Instant 
Returns the ISO 8601 timestamp that the entity was archived at.
#### getArchivedBy(): String 
Returns the user id of who archived the entity.

## ChatEmbed

### Description
TBD

### Methods
#### getTitle(): String
Returns the title of the entity. Maximum length: `256`
#### getDescription(): String
Returns the description of the entity. Maximum length: `2048`
#### getUrl(): String
Returns the url to linkify the title field. Maximum length: `1024`
#### getColor(): Integer
Returns the color of the entity when embed is viewed. Minimum: `0`; Maximum: `16777215`
#### getFooter(): EmbedFooter 
Returns the small section at the bottom of the entity.
#### getTimeStamp(): Instant 
Returns the ISO 8601 timestamp that the entity was set to.
#### getThumbnail(): EmbedThumbnail
Returns the image to the right of the entity's content.
#### getImage(): EmbedImage
Returns the main picture associated with the entity.
#### getEmbedAuthor(): EmbedAuthor
Returns the small section above the title of the entity.
#### getFields(): EmbedField
Returns Table-like cells to add to the entity. Maximum Items: `25` 