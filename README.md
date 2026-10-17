# Tour Campus demo

Open `index.html` in a browser. This standalone prototype uses browser local storage for persistent demonstration data.

It includes Campus, Tour Compute, and Tour Network views. Compute jobs validate predefined safe workloads and resource limits, retain a status history, allocate available demo nodes, support cancellation and simulated failure, store sample output/logs, and record protected single-award demonstration credit entries. The browser demo scopes records to its current demo user.

Network messages use a stored envelope with an ID, sender, recipient, creation/expiry timestamps, hop-limited deterministic route, transport marker, delivery status, and relay history. Topology paths are derived from stored links; peer and gateway availability changes route selection, failures, retries, and expiry. Network topology, peer availability, routes, and messages are simulated; no Bluetooth, compute execution, or monetary credit system is implemented.

Future integration boundaries: an authenticated Compute API backed by a queue, scheduler, isolated worker agents and result storage; and a native mobile networking layer for BLE discovery, authenticated encrypted envelopes, multi-hop routing, expiry, duplicate suppression, consented gateway forwarding, and platform background-operation constraints.
