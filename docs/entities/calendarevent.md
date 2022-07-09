# CalendarEvent

## Getter Methods
### get_JGAPI()
#### JG_API
Returns the instance of JG_API the bot is using.
### getCalendarId()
#### int
Returns the id of the CalendarEvent.
### getServerId()
#### String
Returns the server id of the CalendarEvent.
### getChannelId()
#### String
Returns the channel id of the CalendarEvent.
### getName()
#### String
Returns the name of the CalendarEvent.
### getDescription()
#### String
Returns the description of the CalendarEvent.
### getLocation()
#### String
Returns the location of the CalendarEvent.
### getUrl()
#### String
Returns the URL of the CalendarEvent.
### getColor()
#### int
Returns the color of the CalendarEvent.
### getStartsAt()
#### Instant
Returns the start datetime of the CalendarEvent.
### getDuration()
#### int
Returns the duration of the CalendarEvent.
### isPrivate()
#### boolean
Returns if the CalendarEvent is private or not.
### getMentions()
#### Mentions
Returns the Mentions entity of who is mentioned for the CalendarEvent.
### getCreatedAt()
#### Instant
Returns when the CalendarEvent was created.
### getCancellation()
#### CalendarEventCancellation
Returns the CalendarEventCancellation entity for the CalendarEvent.

## Setter Methods
### setName(String name)
#### RestAction<CalendarEvent>
Will set the name of the CalendarEvent upon completion of the RestAction.
### setDescription(String description)
#### RestAction<CalendarEvent>
Will set the description of the CalendarEvent upon completion of the RestAction.
### setLocation(String location)
#### RestAction<CalendarEvent>
Will set the location of the CalendarEvent upon completion of the RestAction.
### setStart(Instant startsAt)
#### RestAction<CalendarEvent>
Will set the start datetime of the CalendarEvent upon completion of the RestAction.
### setURL(String url)
#### RestAction<CalendarEvent>
Will set the URL of the CalendarEvent upon completion of the RestAction.
### setColor(int color)
#### RestAction<CalendarEvent>
Will set the color of the CalendarEvent upon completion of the RestAction.
### setDuration(int duration)
#### RestAction<CalendarEvent>
Will set the duration of the CalendarEvent upon completion of the RestAction.
### setPrivate(boolean isPrivate)
#### RestAction<CalendarEvent>
Will set the privacy of the CalendarEvent upon completion of the RestAction.
### delete()
#### RestAction<Boolean>
Will delete the CalendarEvent upon completion of the RestAction.
### update(String name, String description, String location, Instant startsAt, String url, int color, int duration, boolean isPrivate)
#### RestAction<CalendarEvent>
Will update the specified fields upon complete of the RestAction.