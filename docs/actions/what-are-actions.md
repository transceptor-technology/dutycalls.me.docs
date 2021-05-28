# What are actions?

When DutyCalls receives a ticket, it checks whether certain actions need to be addressed first. There are three actions:

* **Silence** - the channel participants will not be notified about this ticket.

* **Assignment** - the ticket will be assigned to a provided workspace user.

* **Auto-close** - the ticket will be closed under the name of a provided workspace user.

How does DutyCalls know when to execute these actions? One or more of these three actions can be configured for a certain tag. The corresponding actions will be executed in case a ticket contains that tag.
