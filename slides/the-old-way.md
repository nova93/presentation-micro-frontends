
# The Old Way

#### or the `current` way, depends how much you squint

<br />
<br />

| <strong>Bottlenecks</strong> |  Does/Did it exist? |
|---|:-:|
| <v-clicks at="1"><span>Monolithic Frontend</span></v-clicks> | <v-clicks at="2"><uim-check-circle /></v-clicks> |
| <v-clicks at="3"><span>Monolithic Backend</span></v-clicks> | <v-clicks at="4"><uim-check-circle /></v-clicks> |
| <v-clicks at="5"><span>Unreliable (and long) deployments</span></v-clicks> | <v-clicks at="6"><uim-check-circle /></v-clicks> |

<!-- ./components/SelfPromo.vue -->
<SelfPromo />

<!--
Monolithic Frontend: my-ocf-app

Single team, so there weren't any cross-team issues
A lot of legacy code, hard to remove due to loss of tribal knowledge

As the team grew we started building more stand-alone apps, such as sales tool and ocf.com (migration from wordpress).

At one time, we had 3 separate vehicle search experiences, copy/pasted between apps, some of which were in Javascript, some in Typescript, which made any updates a real pain, and we had a really hard time keeping the experiences the same. As a side note, this is actually why the team eagerly embraced Virtuoso.

---

Monolithic Backend: bobcat and my-ocf-app-service

Two team, native app and web. Two "BFFs", in quotes. Started very well, and until not that long ago, made a weird kind of sense.

However, teams were isolated from each other, and weren't sharing any solutions, which lead to interesting discrepancies, one such discrepancy was how do we pick the most appropriate loan application.

Can't speak for the native apps, since I don't have enough knowledge of their architecture, but for web it quickly grew into a problem.

How would we spin up a new app? We'd copy/paste Elasticbeanstalk terraform, and we'd have 2 apps running in parallel, doing pretty much the same thing.

As the team split and split again, and more devs joined, it quickly became apparent that this is not a scalable model.

---

Deployments

EBS deployment takes around 20mins, usually fails, overall average deployment time around 1 hour. Dev sits there watching the paint dries, so they can manually attempt deployment

Uses Carsnip jenkins - for the longest time, required Carsnip VPN to access.

really old news now, but we used to have s3 website deployments - static only, lack of server-side rendering, requirement to run manually created Lambda@Edge redirect scripts (same for CSPs), all solved with the move to Vercel.
-->
