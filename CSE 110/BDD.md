## Definition
- Behavior driven development
- Turn idea for a requirement into a implemented, tested, production ready code simply and effectively as long as the requirement is specific enough
## Structure
```
Title (one line describing the story)

Narrative:
As a [role]
I want [feature]
So that [benefit]

Acceptance Criteria: (presented as Scenarios)

Scenario 1: Title
Given [context]
  And [some more context]...
When  [event]
Then  [outcome]
  And [another outcome]...

Scenario 2: ...
```
- Title of story should describe an activity
	- "Account Holder withdraws cash"
- Narrative of story is:
	- As a [role] I want [feature] so that [benefit] 
- Scenario title should say what's different between each scenario
- Given [context]
- And [some more context]...
- When [event]
- Then []
## Good vs Bad BDD Scenarios
- Bad:
	- Title is vague
	- Given is vacuous 
	- Underspecified
- Good:
	- For a given user story driven by unique progressions into **and** out of the feature
	- 