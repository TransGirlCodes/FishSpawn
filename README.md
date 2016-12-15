# FishSpawn

A Minitab 12.1 macro written by Cock van Oosterhout to test
the repeatability of mate choice:

To test whether the F2 female spawning pattern deviates significantly from a
random pattern, we simulated a distribution of spawning events of 69 females
that have had ≥ 5 spawning decisions with either a _P. nyererei_ (_Pn_) or
_P. pundamilia_ (_Pp_) male.

In the simulations, each female is given a probability to mate with a _Pn_ or
_Pp_ male equivalent to the proportion of _Pn_ and _Pp_ spawning events
observed. This probability determines her first spawning decision.
However, once a female has been allocated a mate preference, the strength with
which this preference continues to affect subsequent spawning decisions is given
by the following formulas:

$P(x_i = Pn) = Pn + R(1 - Pn)$

$P(x_i = Pp) = Pp + R(1 - Pp)$

Here, $P(x_i = Pn)$ and $P(x_i = Pp)$ are the probabilities of a female spawning
with a _Pn_ and _Pp_ male at the ith spawning decision (i > 1), and _Pn_ and
_Pp_ are the observed proportion of spawning events with a _Pn_ and _Pp_ male, respectively.
_R_ is the repeatability coefficient $(0 ≤ R ≤ 1)$.
With $R = 0$, spawning is “random” and proportional to the observed proportion
of _Pn_ and _Pp_ spawning events.
In this case, female choice will switch randomly between _Pn_ and _Pp_ males.
With $R = 1$, however, spawning choice is fixed and all spawning decisions are
for males of the same species as the first choice.
In this case, females will consistently choose either for a _Pn_ or a _Pp_ male.
With intermediate values of $R$, there is a preference for a species of male,
but this preference will not completely determine a spawning decision.
