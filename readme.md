# Groq API for roblox
how to use:
## Set up
- push down your code 2 lines
- add `_G.apikey="Your GROQ api key"` to first line
- add the code above to second line
## Use
### SetModel
```lua
groq:SetModel(string ModelName)
```
set current model
### SetSystemPrompt
```lua
groq:SetSystemPrompt(string Prompt)
```
Sets current system prompt
### RequestAI
```lua
groq:RequestAI(string message, int32 max_tokens=256, float32 temp=1, int32 seed=os.time(), char stop='')
```
requests ai ticket.
### CreateTool
```lua
groq:CreateTool(string name, string desc, string[] params, string[] required, function callback)
```
creates a tool that can be used by ai.
callback will be called with args returned by ai
### ResetChats
```lua
groq:ResetChats()
```
resets chat history
