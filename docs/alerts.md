# Alerts

## Overview

Would you like to stay up to date on the latest events in a workspace? Make use of alerts. These can be configured globally per workspace or specifically per channel depending on the type of the alert.

---

## Alert types

### Manager alerts

Alerts of this type will be sent to the manager of the channel.

`Number of channel subscribers`
:   This alert will be raised when too few users have subscribed themselves on a particular channel. The minimum number of subscribers can be configured in the **General** section of the channel settings.

`Number of active channel subscribers`
:   This alert will be raised when too few active users have subscribed themselves on a particular channel. The minimum number of subscribers can be configured in the **General** section of the channel settings.

`Ticket unacknowledged too long`
:   This alert will be raised when a ticket has been unacknowledged for too long. This time can be configured globally per workspace or specifically per channel in the **Alerts** section of the settings. The time will be reset when the status of the ticket changes.

`Ticket acknowledged too long`
:   This alert will be raised when a ticket has been acknowledged for too long. This time can be configured globally per workspace or specifically per channel in the **Alerts** section of the settings. The time will be reset when the status of the ticket changes.

`Ticket open too long`
: This alert will be raised when a ticket has been open for too long. This time can be configured globally per workspace or specifically per channel in the **Alerts** section of the settings. The time will be reset when the status of the ticket changes.

`Expectation rule not met`
:   This alert will be raised when an expectation rule has not been met. These expectation rules can be configured in the **Expectations** section of the channel settings.

### Subscriber alerts

Alerts of this type will be sent to the subscribers of the channel.

`Severity threshold exceeded`
:   This alert will be raised when a ticket arrives in DutyCalls with a severity higher than the configured threshold. The threshold can be configured globally per workspace or specifically per channel in the **Alerts** section of the settings.
