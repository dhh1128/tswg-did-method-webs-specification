[[def: superseding-recovery, superseding recovery, superseding recoveries]]

~ KERI's mechanism for recovering control of an AID whose current signing keys
~    have been exploited: a [[ref: rotation event]] accepted at a sequence
~    number already occupied by an earlier event, which supersedes that event
~    and disputes the branch descending from it. The KEL forks at that sequence
~    number by construction, and reconciliation establishes which side is the
~    [[ref: trunk]]. KERI constrains which events may be superseded — a
~    rotation may supersede an [[ref: interaction event]], while a
~    non-delegated rotation may not supersede another rotation, and a
~    delegated rotation is resolved against the delegator's KEL. Read the
~    rules before relying on this summary.

~ More detail: the [KERI specification](#KSWG-KERI), §Superseding Recovery and
~    Reconciliation.
