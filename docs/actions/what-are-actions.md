# What are actions?

When DutyCalls receives a ticket, it checks whether certain actions need to be addressed first.

There are four types of actions:

* **Silence ticket** - the channel participants will not be notified about this ticket.

* **Assignment ticket** - the ticket will be assigned to a provided workspace user.

* **Auto-close ticket** - the ticket will be closed under the name of a provided workspace user.

* **Run HTTP(S) request** - a configured HTTP(S) request will be executed.

How does DutyCalls know when to execute these actions? One or more of these actions can be configured for a certain tag. The corresponding actions will be executed in case a ticket is received containing that tag.
