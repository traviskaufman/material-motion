---
layout: page
---

# A consultation interface

TODO: Spec this out.

A consultation interface is an entity that is able to dispense plans in response to a provided set of "goal" states. This interface might be a *learning* entity and it might be *context-aware*.

    TransitionDirector: Director {
      function setUp(transaction) {
        plans = consultation.describePlansFor(leftState, rightState)
        // Maybe change the plans if we don't like them here.
        transaction.add(plans)
      }
    }
