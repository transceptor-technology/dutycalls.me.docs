# Deduplication

Tired of duplicate tickets? Then use the available deduplication methods.

## Dedup key

For channels with API integrations, if multiple tickets are created for the same issue, your team will be notified for each duplicate ticket. To group these tickets, you will want to include `dedupKey` in your parameters for creating tickets.

DutyCalls de-duplicates incidents based on the `dedupKey` parameter. If there are no open (unresolved) tickets with this key, a new ticket will be created. If there is already an open ticket with a matching key, this event will be appended to that ticket as a hit.
