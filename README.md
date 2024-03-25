# Discounted Brownian Bandits with Normal Beliefs


See the pdf file for a full compiled version.


# Introduction

Learning through experimentation is typically characterized as a
multi-armed bandit problem, where the agents face the decision of
choosing among a set of actions, whose consequences might be contingent
on the state of the world. In the simplest case with two actions, we
refer to the two-armed bandit problem that involves one safe arm with a
known expected payoff and a second risky arm with an unknown expected
payoff that may be higher or lower than the safe payoff. The problem
here is typically portrayed as a trade off between exploiting what we
already know (and is safe) and exploring the condition of something that
might be possibly better than the safe course of action. As opposed to
other types of learning environments, where typically the cost of
information is exogenous, in bandit problems the cost of learning is
simply the opportunity cost of not exploiting the returns of the safe
action. So, one faces the decision of to what degree they should
experiment and when to stop experimenting. Typically, the strategies are
defined as mappings from the belief space to the allocation of a
resource among the actions, where it's assumed that the agent makes her
decision only depending on her current subjective belief of the world.
The strategies are then chosen in order to maximize total expected
payoffs.

Historically, the environment usually involved only a single-agent
acting on her own and only observing her own actions and their
consequences, whereas in the modern literature the strategic
interactions in a social learning environment, allowing agents to learn
from each others' actions is the focal point of the analysis. With the
recent developments, notoriously intractable nature of the bandit
problems are understood to a greater degree. Mainly, we talk about two
effects that evolves from the strategic consideration in a social
learning environment: the free-riding effect and the encouragement
effect. The first is a natural result of the two main properties of the
model: ability to learn from each others' actions and the assumption
that the experimentation procedure and the state of the world is
identical among the agents. This conjunction leads agents to shy away
from costly experimentation as long as they believe that there are other
people, who are undertaking a sufficient amount of experimentation and
(depending on the model) are going to share their experimentation
results fully and truthfully with them. Believing this, agents have no
incentive to undertake costly experimentation, when they can just as
well continue to use the safe arm and be indirectly benefiting from the
experimentation at the same time. The latter effect can also be thought
of as a result of free-riding. Given that incentives to experiment are
problematic and as nobody wants to be the guinea pig of the group,
experimentation process can slow down undesirably, even though it's
beneficial for everyone. Hence, knowing that a good experimentation
outcome today might lead someone to join experimentation tomorrow one
has then the incentive to be the leader of the group to motivate social
welfare. This effect is only sustained if the good news are inconclusive
i.e. when there is still something to learn after a good outcome.
Nevertheless, typically the free-riding effect is still persistent
enough to cause inefficient levels of experimentation. Although, with
recent developments, we see that efficiency is in fact achievable under
different equilibrium considerations.

As a technical simplification, the literature typically treats the
problem in a setting where the state of the world is considered to be
binary: *good* or *bad*. This naturally leads to the conclusion that
prior to conducting experimentation, agents have to know exactly what
two outcomes they might be facing. In an artificial game where rules are
communicated in advance (like a gambling machine) this assumption might
be non-restrictive. Although, as especially in the economics literature
the setup is thought of as an abstraction of real-world experimentation
like drug trials or mineral discoveries; thinking of the state space as
higher dimensional (potentially continuous) should allow for an
environment that is more suitable for real-world justifications, which
may also lead to a more elastic learning environment and higher levels
of efficiency.

A potential benefit of achieving tractable analysis under a continuous
state space might be that, then, the state of the world can be thought
of as the resulting outcome of a completely different non-binary
process. For example, the *goodness* of the arm might be time-dependent.
This might relate to concepts like time-dependent preferences or
external shocks that change the underlying characteristic of payoffs. In
the case of drug trials, the binary setup only allows for whether the
drug is more effective than a benchmark level or not. In a non-binary
state, how effective the drug is can also be characterized in order to
potentially compare with other opportunities like simultaneous
experimentation. Further, the effectiveness of the drug might be
dependent on time-dependent complications with other stimulants and
hence the signal that experimentation produces might also be biased
depending on at which point in time the experimentation is undertaken.
With time dependent tastes, expected benefit of experimentation (and
it's relation to the opportunity cost) can be variable at different
points in time, which might lead to time variable cutoff beliefs that
agents use to decide when to experiment. Such a model might be used to
explain periodic risk sensitives depending on factors like
self-confidence and liquidity.
