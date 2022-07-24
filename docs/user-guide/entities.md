# JG_API Entities
---
Explain what they can expect here...

## CalendarEvent
### Description
The `CalendarEvent` is the entity returned for events `CalendarEventCreatedEvent`, `CalendarEventDeletedEvent`, `CalendarEventUpdatedEvent`.
### Methods

#### Getter
##### getCalendarId(): Integer
Returns the id of the entity.
##### getServerId(): String
Returns the server id of the entity.
##### getChannelId(): String
Returns the channel id of the entity.
##### getName(): String
Returns the name of the event. Minimum length: `1`; Maximum length: `60`
##### getDescription(): String
Returns the description of the event. Minimum length: `1`; Maximum length: `8000`
##### getLocation(): String
Returns the location of the event. Minimum length: `1`; Maximum length: `8000`
##### getUrl(): String
Returns the URL to associate with the event.
##### getColor(): Integer
Returns the color of the event when viewed in the calendar. Minimum: `0`; Maximum: `16777215`
##### getRsvpLimit(): Integer
Returns the number of RSVPs to allow before waitlisting RSVPs. Minimum: `1`
##### getStartsAt(): Instant
Returns the ISO 8601 timestamp that the event starts at.
##### getDuration(): Integer
Returns the duration of the event in minutes. Minimum: `1`
##### isPrivate(): Boolean
Returns if the CalendarEvent is private or not.
##### getMentions(): Mentions
Returns the Mentions entity of the CalendarEvent entity.
##### getCreatedAt(): Instant
Returns the ISO 8601 timestamp that the event was created at.
##### getCreatedBy(): String
Returns the ID of the user who created this entity.
##### getCancellation(): CalendarEventCancellation
Returns the CalendarEventCancellation entity.

#### Setter
##### setName(String name): RestAction<CalendarEvent>
Creates a RestAction where the name will be set to the specified String `name` parameter.
##### setDescription(String description): RestAction<CalendarEvent>
##### setLocation(String location): RestAction<CalendarEvent>
##### setStart(Instant startsAt): RestAction<CalendarEvent>
##### setUrl(String url): RestAction<CalendarEvent>
##### setColor(int color): RestAction<CalendarEvent>
##### setDuration(int duration): RestAction<CalendarEvent>
##### setPrivate(boolean isPrivate): RestAction<CalendarEvent>
##### delete(): RestAction<CalendarEvent>
##### update(String name, String description, String location, Instant startsAt, String url, int color, int duration, boolean isPrivate): RestAction<CalendarEvent>

## CalendarEventCancellation