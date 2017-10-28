["@homepage": "https://werewolf.world"](https://werewolf.world)

"version": "0.1"

# Examples

## Entity list

|Entity list|JSON-LD|
---|---
|all-agents|[https://werewolf.world/example/0.1/all-agents.jsonld](https://werewolf.world/example/0.1/all-agents.jsonld)|
|all-roles|[https://werewolf.world/example/0.1/all-roles.jsonld](https://werewolf.world/example/0.1/all-roles.jsonld)|

## System outline

<a href="https://werewolf.world/diagram/0.1/werewolf_system_outline.svg" target="_blank">![system outline](https://werewolf.world/diagram/0.1/werewolf_system_outline.png)</a>

## Server-to-client message examples

|Example|JSON-LD|
---|---
|first-day-conversation|[https://werewolf.world/example/0.1/server2client/first-day-conversation.jsonld](https://werewolf.world/example/0.1/server2client/first-day-conversation.jsonld)|
|day-conversation|[https://werewolf.world/example/0.1/server2client/day-conversation.jsonld](https://werewolf.world/example/0.1/server2client/day-conversation.jsonld)|
|day-vote|[https://werewolf.world/example/0.1/server2client/day-vote.jsonld](https://werewolf.world/example/0.1/server2client/day-vote.jsonld)|
|night|[https://werewolf.world/example/0.1/server2client/night.jsonld](https://werewolf.world/example/0.1/server2client/night.jsonld)|
|results|[https://werewolf.world/example/0.1/server2client/results.jsonld](https://werewolf.world/example/0.1/server2client/results.jsonld)|
|post-mortem|[https://werewolf.world/example/0.1/server2client/post-mortem.jsonld](https://werewolf.world/example/0.1/server2client/post-mortem.jsonld)|
|my-message-on-chat|[https://werewolf.world/example/0.1/server2client/my-message-on-chat.jsonld](https://werewolf.world/example/0.1/server2client/my-message-on-chat.jsonld)|
|their-message-on-chat|[https://werewolf.world/example/0.1/server2client/their-message-on-chat.jsonld](https://werewolf.world/example/0.1/server2client/their-message-on-chat.jsonld)|
|error|[https://werewolf.world/example/0.1/server2client/error.jsonld](https://werewolf.world/example/0.1/server2client/error.jsonld)|

### first-day-conversation

* "Start day conversation phase" to "Display" and "Move to grave"

### day-conversation

* "Start day conversation phase" to "Display" and "Move to grave"

### day-vote

* "Start day vote phase" to "Display" and "Move to grave"

### night

* "Start night phase" to "Display" and "Move to grave"

### results

* "Send results" to "Display results in a modal"

### post-mortem

* "Start post mortem phase" to "Display"

### my-message-on-chat

* "Broadcast a chat message" to "Display a chat message"

### their-message-on-chat

* "Broadcast a chat message" to "Display a chat message"

### error

* ("Server error" in server to "Output a log" in server and "Show an error message" in client)

## Client-to-server message examples

|Example|JSON-LD|
---|---
|board|[https://werewolf.world/example/0.1/client2server/board.jsonld](https://werewolf.world/example/0.1/client2server/board.jsonld)|
|chat|[https://werewolf.world/example/0.1/client2server/chat.jsonld](https://werewolf.world/example/0.1/client2server/chat.jsonld)|
|day-vote|[https://werewolf.world/example/0.1/client2server/day-vote.jsonld](https://werewolf.world/example/0.1/client2server/day-vote.jsonld)|
|night-vote|[https://werewolf.world/example/0.1/client2server/night-vote.jsonld](https://werewolf.world/example/0.1/client2server/night-vote.jsonld)|
|scroll|[https://werewolf.world/example/0.1/client2server/scroll.jsonld](https://werewolf.world/example/0.1/client2server/scroll.jsonld)|
|error|[https://werewolf.world/example/0.1/client2server/error.jsonld](https://werewolf.world/example/0.1/client2server/error.jsonld)|

### board

* "Update prediction board" to "Output a log"

### chat

* "Send a chat message" to "Receive a chat message" in both Day Conversation Phase or Post Mortem Phase

### day-vote

* "Vote" to "Collect votes" in Day Vote Phase

### night-vote

* "Vote" to "Collect votes" in Night Phase

### scroll

* "Scroll" to "Output a log"

### error

* ("Client error" in client to "Output a log" in server and "Show an error message" in client)