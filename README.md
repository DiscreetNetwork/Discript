# The Actor Model - Primer

The actor model is a mathematical model of concurrent computation that treats actor
as the universal primitive of computation. In response to a message, an actor can:

- Create a finite number of new actors
- Send a finite number of messages to other actors
- Update it's own local state

There is no assumed sequence to the above actions, nor is it assumed that
messages will arrive in any particular order. However, it is required that
messages are processed in a manner that is fair, and the network must guarantee
eventual service.

The actor model is turing-complete. Not only that, it is entirely irrelevant what
actors and messages are!

Our actors might as well be points in a directed graph, and messages be a
signal that carry no information. The model remains turing-complete as long as
the graph can have cycles, and nodes can have at least two children.


# The Actor Model and Discript

A Discript program can have one or more actors. The actors are compiled into
arithmetic circuits, which can be "evaluated" as a bulletproof, producing a proof
of execution.

Arithmetic circuits are equivalent in power to a lookup table, or a pure, stateless,
total function. This makes them quite limited from a programmer's perspective.

It would be possible for Discreet to store local state on the Paranet, which
would make actors equivalent in power to a DFA or FSM.

TODO: Actors can communicate across programs
