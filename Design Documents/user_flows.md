# User flows

### Flow 1: check how often a plant needs to be watered
- Ask Alexa how often a specific plant needs to be watered (user needs to know the plant species and give this info to Alexa in the question)
- Alexa gets the information either by
  - Checking an existing database of plants and watering needs
  - Searching the internet / from an API to answer the question
- Alexa returns the information very succinctly

### Flow 2: set up a recurring reminder to water a new plant
- Ask Alexa to remind you to water a specific plant
- Alexa checks if you have any existing reminder for this plant
- You confirm to Alexa when you last watered this plant
- Alexa sets a recurring reminder starting for the number of days in the future that plant needs to be watered - the days since you last watered

### Flow 3: check when a plant was last watered
- Ask Alexa when a specific plant was last watered (assume only one of each species of plant / they will always be watered together)
- Alexa checks scheduled reminders for the species of this specific plant (e.g. water Monstera)
- Alexa uses the number of days remaining on this reminder to back calculate when it was last watered
- Alexa tells you if the watering is overdue or if not overdue when it was last watered and the schedule for watering this plant
- If watering is nearly due then remind the user how to check if it needs watering

### Flow 4: tell Alexa a plant has been watered & reset upcoming reminders
- Tell Alexa that a specific plant has been watered
- Alexa cancels upcoming reminders and resets based on the number of days to when it will need watering again

### Flow 5: integration to routines, e.g. dismissing a morning alarm reads out which plants need to be watered today
- Edit existing alarm dismissal routine to activate this skill and check if any reminders are upcoming today to water plants
- Note: this may be possible with existing reminder functionality, if yes, prefer built-in functionality
