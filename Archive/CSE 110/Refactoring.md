## Definition
- Changes to the internal structure of your code without affecting the code behavior usually related to a *specific improvement in your design*

## Example 
- Changing the `getDisabilityAmount` method from several if statements that check seniority and months disabled by making a new method called `isEligibleForDisability()` and simply calling that each time in `getDisabilityAmount`
	- Goal was to make updating future disability requirements easier