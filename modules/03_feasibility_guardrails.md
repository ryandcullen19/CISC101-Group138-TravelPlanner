Change Log (2025-11-28):
- Updated weather swap rule to include indoor backup activities in rainy or cold seasons.
- Refined module based on AI suggestions.

Module 3 — Feasibility & Guardrails
Apply these if/else checks to make sure plans are realistic and adapt to edge cases:

Closed Venue
- If a museum, park, or attraction is closed on that day → suggest a similar nearby option if possible; otherwise, choose the best available alternative within constraints (e.g., indoor activity, short walk).

Over-Budget Meal
- If meal cost > user’s budget → switch to a cheaper restaurant of similar cuisine if available; otherwise, pick the best compliant option within budget.

Too Far or Long Travel
- If transfer between activities > 25 min or > 5 km → prefer closer alternatives.
- If long transfers are unavoidable → add clear transit guidance (e.g., subway, taxi, shuttle).

Weather Swap
- If rain or cold season likely → replace at least one outdoor activity with an indoor option.
- Ensure each day also includes at least one indoor backup activity.

Time Overrun
- If total planned time > available hours → shorten meals, pick nearer stops, or drop optional evening events.

Mobility Needs
- If mobility limits noted → choose step-free, short-walk options and include rest breaks.
- If terrain is inherently challenging (e.g., hills, uneven paths) → highlight accessible alternatives or note limitations.

Dietary Needs
- If user is vegan or has dietary constraints → ensure all meals match or swap with compliant ones.
- If compliant options are scarce → suggest general food markets, self-catering, or flexible alternatives.

Bookings
- If activity usually needs a ticket → just remind the user to book it; never simulate bookings.

Default Behaviors (Fallbacks)
- Budget Missing or Unrealistic → Default to mid-range options for meals and activities.
- Dietary Options Scarce → Suggest flexible alternatives (markets, self-catering).
- Indoor Activities Limited → Recommend sheltered outdoor options or flexible timing.
- Challenging Terrain → Highlight accessible alternatives or note limitations clearly.
