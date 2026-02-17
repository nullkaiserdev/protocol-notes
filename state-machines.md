# State Machines in Protocol Design

Protocols are state machines first, and applications second.

Every critical bug I’ve seen can be traced to one of:
- Invalid state transitions
- Missing invariants
- Assumed ordering that was never enforced

Design starts by answering:
- What states are allowed?
- Who can move the system between them?
- What must always be true, regardless of inputs?

If these are not explicit, the protocol is already broken.
