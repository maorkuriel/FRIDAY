# Experimentation & A/B Testing - Knowledge Base

> Curated from 22+ episodes of Lenny's Podcast

## Frameworks

### 1. Overall Evaluation Criterion (OEC) - Ronny Kohavi

Define what you're actually optimizing for. Rather than a single metric like revenue (which can be gamed), combine a primary metric with guardrail metrics. At Bing, revenue with constraints on page real estate prevents plastering ads everywhere.

*Source: episodes/ronny-kohavi*

### 2. Explore and Exploit - Albert Cheng (Duolingo, Grammarly, Chess.com)

Two phases of growth experimentation:
- **Exploration:** Find winning patterns (what resonates with users)
- **Exploitation:** Scale those winners across the product

Teams oscillate: discover a winning insight, amplify it, then return to exploration when exploitation plateaus.

*Source: episodes/albert-cheng*

### 3. Evidence-Guided Decision Making - Itamar Gilad

Balance human judgment with data using GIST (Goals, Ideas, Steps, Tasks) and metrics trees. Gmail's tabbed inbox succeeded because teams tested rigorously instead of assuming.

*Source: episodes/itamar-gilad*

### 4. Twyman's Law - Ronny Kohavi

If a result looks too good to be true, it probably is. When normal improvements are under 1% but you suddenly see 10% gains, investigate. Kohavi found flaws 9 out of 10 times when applying this law.

*Source: episodes/ronny-kohavi*

### 5. Build-Measure-Learn - Eric Ries

The fundamental experimentation loop: form a hypothesis, build the minimum viable version, measure results, learn. This is descriptive -- it names what successful startups already do -- not prescriptive dogma.

*Source: episodes/eric-ries*

---

## Best Quotes

> "I'm very clear that I'm a big fan of test everything. Any code change, any feature that you introduce has to be in some experiment. Even small bug fixes can sometimes have surprising, unexpected impact."
> -- Ronny Kohavi

> "Of these experiments, 92% failed to improve the metric that we were trying to move. So only 8% of our ideas actually were successful."
> -- Ronny Kohavi

> "If you go for something big, try it out, but be ready to fail 80% of the time."
> -- Ronny Kohavi

> "The typical win rate for experiments is often something like 30 to 50%. Consumer products are very unpredictable like that, but when you do find a thing that breaks through the noise, it could actually be a hugely losing experiment too -- those are also super valuable."
> -- Albert Cheng

> "MVP is simply for whatever the hypothesis is that we're trying to test, what is the most efficient way to get the validation we need?"
> -- Eric Ries

---

## Common Mistakes

1. **Launching full redesigns without incremental testing.** Every time Kohavi has seen large product redesigns, they've failed dramatically. Decompose into small, testable changes. (Ronny Kohavi)

2. **Not documenting learnings.** Companies run lots of experiments and never summarize. Teams repeat the same failed experiments. Microsoft ran 20,000+ experiments per year but had to explicitly build documentation systems. (Ronny Kohavi)

3. **Misunderstanding p-values.** A p-value of 0.05 does not mean 95% probability the treatment is better. When success rates are low (like Airbnb's 8%), a "significant" result can still have a 26% false positive rate. (Ronny Kohavi)

4. **Building on opinion instead of evidence.** Google+ had 1,000+ engineers building on conviction. Gmail's tabbed inbox had a small team testing rigorously. Conviction without validation is dangerous. (Itamar Gilad)

---

## Company Examples

**Bing** (Ronny Kohavi): A simple experiment moving the second ad line to the first increased revenue by 12% -- worth $100M. Nearly dismissed because it seemed trivial. Proves how hard it is to predict outcomes.

**Netflix** (Gibson Biddle): "Perfect New Release" test showed minimal retention improvement (4.5% to 4.45%) despite being what customers asked for. Revealed the real value prop wasn't speed but variety.

**Chess.com** (Albert Cheng): Found 80% of users review games after wins, not losses. Changed messaging to highlight brilliant moves instead of blunders. 25% increase in game reviews, 20% in subscriptions.

**Grammarly** (Albert Cheng): Free users thought it was just spelling/grammar. Interspersing paid suggestions into the free experience (a "reverse free trial") nearly doubled upgrade rates.
