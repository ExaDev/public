---
title: Universal Filter Board
aliases:
  - Universal Filter Breadboard
tags:
  - breadboard
  - breadboard/phase/2
created: 2024-06-21T08:19:04
modified: 2024-06-21T08:41:23
---

Inspired the concept of the [Placeholder Board](projects/Breadboard/Phase%202/boards/Placeholder%20Board.md) as the "logic" / "wiring" could be written already

1. **Concept:**
	- Implement a filtering mechanism using a Large Language Model (LLM).
	- Process an array of inputs based on defined filtering criteria.
2. **Workflow:**
	- Input Processing:
		- Receive an array of inputs and apply filtering criteria.
		- Filtering criteria defined by the LLM prompt
	- LLM Decision-Making:
		- Incrementally process inputs, making accept/reject decisions.
	- Feedback Loop:
		- Use decisions to refine subsequent choices by feeding back into the LLM.
	- Each result has:
		- Decision
		- Rationale
		- Certainty?
1. **Features:**
	- Pre-seeding:
		- Option to initialise the LLM with predefined accepted and rejected items and candidates.
		- Adaptive Filtering:
			- LLM adapts its filtering based on feedback from previous decisions.
	- Training wheels
		- After each decision user can modify the `Decision`, `Rationale` and `Certainty` values before it is fed back into the LLM to make the next choice
2. **Design Considerations:**
	- Criteria Definition:
		- Clearly define the filtering criteria for the LLM.
		- Decision Feedback:
			- Implement a robust feedback mechanism to enhance decision accuracy.
3. **Next Steps:**
	- Develop a prototype of the universal filter board.
	- Define and integrate filtering criteria.
	- Implement feedback loop functionality.
	- Test with a diverse set of input data to validate effectiveness and adaptability.