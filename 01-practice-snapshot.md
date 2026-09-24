Pre-existing background material of the author. First published 2026-09-24 as release package-v1.0.1 at https://github.com/thoughtform-co/practice-snapshot/releases/tag/package-v1.0.1. Cite entries by their BG id.

# The practice, in thirteen sections

## 0. What this is

A snapshot of how one intelligence architect works, written for people who will work beside him and for the assistants they set up. It states principles and the words the practice uses for them. It gives one plain example per principle and then stops. It does not carry the mechanics behind the principles, the tooling, or any client's material. Those turn an idea into a delivery; they are engagement work, built with each team, in that team's tools, under that team's ownership.

Every section carries an id in brackets. The manifest beside this file says where each idea was first written down and when. Cite the id, say the idea in your own words, and the provenance stays clear for everyone.

## 1. Intelligence is a resource the organisation already runs on [BG-01]

A company meters electricity in kilowatt-hours, storage in gigabytes and people in hours. It meters intelligence in tokens, and a token says how much was asked, never whether the answer was good or who checked it. That is the first fact of the work: there is no unit of useful intelligence, and none is coming. So the resource is managed through the work rather than through the meter. The operating question is not "how many tokens did the marketing team use" but "which pieces of marketing work now run on a model, on what setup, and with what result".

Example: two teams of the same size, and one uses ten times more than the other. Read as a meter, one team is expensive. Read as work, the expensive team moved its weekly report from two people and a day to a model and an hour of review, and the review is where the value now sits. The number was never the finding; the workflow was.

## 2. Between a tool and a collaborator [BG-02, BG-03]

A tool does what it is told. A colleague reads the situation, fills in what was left out and decides how much to decide. A language model does both at once, which is why neither habit fits it. Treated as software it disappoints, because it interprets. Treated as a person it disappoints, because it forgets, varies and cannot be held to account. The practice's answer is a third posture: brief it, calibrate how much freedom it gets, judge what comes back. That loop is the basic unit, and everything else in this document is that loop made durable.

The real question behind every "which model should we use" is therefore how intelligence should take part in a given piece of work. Once that is answered, the model is one field in the answer.

Example: an HR team asks which model to buy. The useful first hour is spent not on models but on their job-description review: what a good review looks like, which parts are mechanical and which need a recruiter's judgment. The model choice falls out of that in five minutes.

## 3. The unit of design is the configuration, not the model [BG-04]

For one piece of work, the configuration answers six questions. What runs it: the model, the skill, the tool. What it inherits: the context, the examples, the judgment it starts from. What it can reach: systems, data, connectors, which is where the data red lines live. How much it decides alone, and where a person reviews. Who owns it: the maintainer, and the person accountable for the outcome. And the bar: how anyone knows the output was good. A configuration is something a leader can govern and an engineer can build against; a model name is neither.

Example: "we use the assistant for product descriptions" is not a configuration. "Product descriptions run on the everyday model, from the brand rules and six approved examples, reading the product sheet, drafting only, reviewed by the copy lead, owned by her, checked against four cases" is one, and it can be costed, audited and improved.

## 4. Where the person sits [BG-05]

Every recurring piece of work gets one of three seats. Execute: the shape is known, the model runs, a person checks, and the check is fast because the shape was fixed before the run. Contribute: the work is still being thought, the model drafts an angle or argues the other side, and a person is in the exchange the whole way. Defer: the team keeps the work, because it is a judgment call, a relationship or a decision that carries a name.

Mapping every recurring piece of work onto those seats, in the open, with the people who do it, is unglamorous and is the whole game. The map that results is more than a catalogue of what runs on a model. Its value is the negative space: what stays deliberately person-led, what was tried and rejected, what is not covered yet.

Example: a support team maps its recurring tasks. About a third execute, a quarter contribute, the rest defer. The deferred list is the first thing the head of support shows the board, because it is the list nobody else can produce.

## 5. Context is rules, examples, sources and loops [BG-06]

Ask a good team how they know a brief is right and you get a look, not a sentence. That knowledge is real and it lives nowhere: in who reviews what, in the examples people reach for, in the three things a senior person always catches. Writing it down is called encoding, and the written form is a layer with four parts. Rules: the constraints that never move, short and boring. Examples: three good ones beat a page of description, because a model, like a new colleague, learns the shape from the specimen. Sources: where the facts come from, named, so the model stops inventing. Loops: who checks, against what, and what a revision may change. The layer is the team's, not the vendor's. It works from any model, survives a model change and belongs to the people who wrote it.

Example: a brand's tone guide is forty pages. The encoded layer is one page of rules, three approved pieces, the product sheet as the only source of claims, and a two-step review. The forty pages stay as background; the one page is what runs.

## 6. Encode the settled part, leave the live edge [BG-07]

Only judgment that has stopped changing is worth writing down. Judgment that still shifts with each case stays with the expert, who also keeps the settled part current. Two consequences follow. The layer holds what good looks like; the data layer holds what is true. Definitions, entities and facts belong in the data, never frozen inside a skill. And stiffer encoding decays faster: a frozen template or dataset ages with every model release, while a readable, editable rule keeps its value. Scaffolding built around a model's current weaknesses wears out; local judgment does not.

Example: a pricing team encodes its discount rules and, separately, its list of customers. The rules go in the layer; the list stays in the CRM the layer reads. Six months later the list has changed a hundred times and the rules twice.

## 7. Every step declares its freedom [BG-08]

For each step of an encoded workflow, say how much room the model has: fixed (retrieve and check, no variation), adapt (apply the rules to this case, vary within them) or free (options, trade-offs, deliberate divergence). Then say what must never be invented and gets flagged to a person instead: a number, a legal claim, a customer fact. Output produced with freedom is re-checked at a fixed step before it is used. A workflow whose steps all carry the same freedom has not been designed.

Example: a product description. Fixed: the specifications, read from the sheet. Adapt: the tone, from the rules and examples. Free: the opening line, three options. Flagged: any comparative claim against another brand.

## 8. Evals: say where it should go, then check where it arrives [BG-09, BG-15]

An instruction is an aim. A check is a measurement of the landing. Teams that only write instructions never find out. Three reasons the check is not optional: a model differs from run to run, it hides its reasons, and it errs without warning, so it can pass on Monday, fail on Tuesday and sound confident both days. Software fails the same way twice; a model does not.

An eval, at the level of ideas, is three things written down. Cases: real inputs with the answer each must get, drawn from the team's own good and bad examples. Checks: questions a reader can answer yes or no about an output. Gates: what happens when a check fails, which is one of pass, review or block. The owner of the work writes the cases, because the point of a case is that the owner can read it, argue with it and change it. When a check and the owner's considered judgment disagree, fix the check. Show each check failing once, so the team has seen what it catches. And remember that what gets rewarded gets learned, by a model in training and by a team in a review loop alike: a check that rewards the wrong thing teaches the wrong thing.

The same try, grade, adjust loop runs at three scales: a team on its skill, a lab on its model, a field on its practice. The loop is one size; only what gets adjusted changes.

Example: a support team writes four checks for a drafted reply: the answer cites the policy page, the tone rule holds, no refund is promised, the ticket number is untouched. Every draft runs through them. The first week, the tone check fires on every reply to one region, and the team learns the rule was written for one market's register, not that the drafts were wrong. They fix the check.

## 9. Frontier first to learn, fit for purpose to run [BG-10]

New and ambiguous work gets the strongest sensible model with no anxiety about cost, because the expensive failure is caution: a team that rations intelligence uses it less and worse. Work moves to a lighter setup only once it is stable and passes its cases, never as a blanket instruction and never as a saving announced before it is measured. The evals are what make the move safe.

Example: a first pass at job-description reviews runs on the frontier model for a month. Once it clears its cases reliably, the team tries the everyday model on the same cases and reads what changed, out loud, before deciding. Whatever it decides, the difference is visible rather than assumed.

## 10. The definition of done for an encoded asset [BG-11]

An encoded asset counts as done when it carries five things. Explicit freedom per step. A clean boundary between facts and judgment, with facts in the data layer. At least two runnable cases drawn from the owner's real good and bad examples, written with the owner. A named owner and a review rhythm. Conditional rules rather than frozen ones: where the owner exercises judgment, license the judgment ("when X, weigh Y") instead of freezing one answer. Missing one of these, it is a draft. The test behind all five: it survives its builder. It keeps performing, can be understood and can be improved when the person who made it is no longer in the room.

Example: a colleague builds a meeting-notes assistant and leaves. If it has an owner, two cases and readable rules, the next person runs it on Monday. If it has a clever prompt and nothing else, it is gone by Friday.

## 11. Adoption and automation are one flywheel [BG-12]

Adopt: people use the intelligence on real work, not sandboxes. Navigate: the people inside the work learn what it is good for, where it fails and what to ask, and they surface the real use cases, because only they can. Encode: the repeatable part of their judgment gets captured so colleagues can run it. Build: what is encoded and used shows what deserves proper engineering. Each step creates the conditions for the next, different people own different steps, and skipping the encode step is why most enablement gains die with the individual.

Some spend compounds: encoded judgment, cases, corrections, reusable context, bought once and drawn on repeatedly. The rest evaporates: a prompt and a response that disappear. A programme that measures only spend and value cannot tell the two apart and under-invests in the half that compounds. The countable version for any readout: of the work now running on a model, how much reused something that already existed. Reuse is the one line that improves over time. And encoding ratchets: the cost of encoding a shape falls on the first piece of work that needs it, and every later piece inherits it, so each new workflow starts closer to done.

Example: the first team to encode a brand's tone pays for it. The fourth team to need the tone gets it on day one and spends its time on its own judgment instead.

## 12. The handover [BG-13]

An engagement is finished when three things stay behind, and all three are needed: the encoded layer, meeting the standard above; the map, saying which work runs on which setup, who owns it and what stays deliberately person-led; and a team able to extend both. A team with only the map has routing with nothing underneath. A team with only the layer has judgment with nowhere to run it. The consultant's stance follows from this: the pen stays with the team. Bring the method, write the first case together from one real good example and one real bad one, then hand the pen over. An asset whose accuracy depends on the consultant's presence is work that never finished. The engagement is temporary by design, and the test of a good one is that the next case runs without the consultant.

Two habits keep the stance honest. Outsource the thinking, never the understanding: everything a model returns is vetted for whether the person would stand behind it. And name what stays human out loud, in the roadmap, next to the automations. It reads as discipline because it is.

Example: at the end of a sprint the team presents its own assets to its own leadership. The consultant is in the room and says nothing. That is the deliverable.

## 13. What this snapshot is not

It is not the practice's mechanics, its tooling, or any client's material. Those are not here, and their absence is deliberate: they are engagement work, built with each team in that team's tools, and owned there.

To cite an idea from this document, use its id and say the idea in your own words. The manifest beside this file records where each idea was first written down and when.

### Reading list

Public sources the practice reads and points teams to. By title, publisher and year; add your own.

- Building effective agents, Anthropic, 2024.
- Measuring AI ability to complete long tasks, METR, 2025.
- Co-Intelligence: Living and Working with AI, Portfolio, 2024.
