---
layout: archive
title: "Research Workflow"
permalink: /workflow/
author_profile: true
use_math: true
---

{% include base_path %}

<div class="hero-section hero-section--page-intro">
  <p class="hero-eyebrow">Using LLMs for research &middot; York University lecture, 2026</p>
  <p class="hero-tagline">I run my cosmology analyses as large, reproducible computational pipelines &mdash; and I use language models as reviewers and engineering assistants within them, with every result verified and authored by me.</p>
  <p class="hero-position">A short tour of how I work with these tools, and where I don't.</p>
</div>

<div class="research-nav">
  <a href="#engage">How I engage</a>
  <a href="#workflow">The workflow</a>
  <a href="#care">Using them with care</a>
  <a href="#lecture">The lecture</a>
</div>


<div id="engage" class="research-section research-section--flush" markdown="1">

## How I engage with these tools

<p class="research-intro">Getting reliable work from a model whose behaviour shifts with the way you ask comes down to three habits: phrase and format deliberately, learn where the model fails, and hand the failing part to a tool that doesn't.</p>

A language model places every word in a learned landscape, and the prompt decides where you start and which way you move. Phrasing is not cosmetic — in the models I tested for the 2026 lecture, two formats of the same question could shift its accuracy substantially — so I treat prompt design as part of the method.

<img src="/images/llm_probability_landscape.png" class="img-wide" alt="A token probability landscape: related words cluster into bright peaks (physics terms, names, math symbols, everyday words); a marked start point in the physics-terms region shows where a physics-style prompt begins">
<p class="research-block__caption">A sketch of the idea: related words cluster into regions, and the prompt sets where the model begins. Good prompting is steering within this landscape.</p>

Most of a model's well-documented failures — arithmetic, recall, rigid formatting, checking its own work — share one fix: stop asking the model to do the part it is bad at, and give it a tool that is good at it.

<div class="map-list" markdown="0">
  <div class="map-row">
    <div class="map-row__from">arithmetic &middot; bookkeeping</div>
    <div class="map-row__arrow">&rarr;</div>
    <div class="map-row__to"><strong>code execution</strong><span>the runtime does the maths, not the model</span></div>
  </div>
  <div class="map-row">
    <div class="map-row__from">recall from memory &middot; stale facts</div>
    <div class="map-row__arrow">&rarr;</div>
    <div class="map-row__to"><strong>search &amp; retrieval</strong><span>look it up instead of trusting the weights</span></div>
  </div>
  <div class="map-row">
    <div class="map-row__from">free-text formatting &middot; paraphrase drift</div>
    <div class="map-row__arrow">&rarr;</div>
    <div class="map-row__to"><strong>typed / schema'd output</strong><span>the shape is validated; the content is still checked</span></div>
  </div>
  <div class="map-row">
    <div class="map-row__from">checking its own answer</div>
    <div class="map-row__arrow">&rarr;</div>
    <div class="map-row__to"><strong>a separate reviewer</strong><span>a differently prompted check you can read back, step by step</span></div>
  </div>
</div>

</div>


<div id="workflow" class="research-section" markdown="1">

## The workflow

<p class="research-intro">A chatbot answers a message; an agent runs a loop — it plans, acts with tools, reads the result, and continues toward a goal it can check. Agents earn their keep exactly where research lives: multi-step work spanning code, notebooks, and writing, where every step can be verified.</p>

I structure that loop the same way each time, and I keep planning and doing apart:

<div class="flow" markdown="0">
  <span class="flow-step">scope</span>
  <span class="flow-arrow">&rarr;</span>
  <span class="flow-step flow-step--loop">plan &#8646; iterate</span>
  <span class="flow-arrow">&rarr;</span>
  <span class="flow-step">implement</span>
</div>

The model first reads the relevant code and *reports its understanding back to me* before touching anything; we agree a plan; only then does it write. Nothing important changes without that round-trip.

The useful artifact is not just the patch, but the audit trail around it: the files it read, the diff it produced, the tests or reruns that checked it, and the remaining assumptions I still have to inspect myself.

Every non-trivial change is then read by a **panel of small, single-purpose reviewers**, each with its own brief, whose findings a manager reconciles into one recommendation:

<div class="role-grid" markdown="0">
  <div class="role-card"><h4>debugger</h4><p>catches bugs and breaking changes after every edit</p></div>
  <div class="role-card"><h4>skeptic</h4><p>scrutinises significant decisions; assumes hidden debt</p></div>
  <div class="role-card"><h4>conservator</h4><p>flags unnecessary complexity; defends the working code</p></div>
  <div class="role-card"><h4>revolutionizer</h4><p>asks whether a quick patch is hiding a deeper problem</p></div>
  <div class="role-card"><h4>tone &middot; narrative</h4><p>keep prose in my own voice and claims consistent across drafts</p></div>
  <div class="role-card"><h4>manager</h4><p>reconciles the panel into a single, decisive recommendation</p></div>
</div>

Finally, the project keeps **its own memory**: after a notable session the assistant records what was found and decided, and later sessions re-read it before starting. The reasoning accumulates across months instead of resetting with each new conversation. I keep sensitive or unpublished details out of tools unless I control where that context runs. *(This website is maintained the same way.)*

That boundary — work that loops and can be checked — is where I let them help, and where I don't.

</div>


<div id="care" class="research-section" markdown="1">

## Using them with care

<p class="research-intro">These tools amplify what you can do — and what you can get wrong; the faster one lets you move, the more discipline it takes. Five rules keep the science mine:</p>

<div class="principle" markdown="0"><div class="principle__n">1</div><div class="principle__body"><strong>Verify everything you accept.</strong><span>Read the code, re-run the test, sanity-check the number. A confident tone is not a check.</span></div></div>
<div class="principle" markdown="0"><div class="principle__n">2</div><div class="principle__body"><strong>Stay the author.</strong><span>The tool is an instrument; the work is mine. It does not decide what counts as a result or what to claim from it.</span></div></div>
<div class="principle" markdown="0"><div class="principle__n">3</div><div class="principle__body"><strong>Don't outsource understanding.</strong><span>If I can't walk through every step, I don't own it. An agent can build a pipeline; I still have to know it.</span></div></div>
<div class="principle" markdown="0"><div class="principle__n">4</div><div class="principle__body"><strong>Mistrust the confidence.</strong><span>Models sound certain even when wrong. Outputs are drafts, not conclusions; doubt is part of the workflow.</span></div></div>
<div class="principle" markdown="0"><div class="principle__n">5</div><div class="principle__body"><strong>Slow down at the result.</strong><span>Iteration speed is the trap. A headline number deserves the most scrutiny, not the least.</span></div></div>

Used this way, the panel mostly catches the unglamorous errors that are easy to miss by eye — a formula or dimensional slip, a unit or sign convention, a configuration drifted out of sync — and pushes back when a conclusion outruns its evidence. The point is not speed; it is a higher standard, held consistently.

</div>


<div id="lecture" class="research-section" markdown="1">

## The lecture

<p class="research-intro">I gave a lecture on this at York University in 2026 — first building intuition for how these models work, then walking through how I use them in day-to-day research.</p>

<div class="role-grid role-grid--advice" markdown="0">
  <div class="role-card"><h4>Part I &middot; how these models work</h4><ul class="lecture-list"><li>next-token prediction as sampling from a learned distribution &mdash; and how a prompt reshapes it</li><li>the sampling-temperature knob: order versus disorder, through a physicist's lens</li><li>the well-documented failure modes &mdash; arithmetic, recall, formatting, self-checking, long-context drift</li></ul><p class="lecture-takeaway">You leave able to read a model's behaviour, not just use it.</p></div>
  <div class="role-card"><h4>Part II &middot; putting them to work</h4><ul class="lecture-list"><li>agents versus chatbots, and the scope &rarr; plan &rarr; implement loop</li><li>handing the failing part to a tool that doesn't &mdash; code, search, schemas</li><li>review as a discipline: panels of differently-motivated checks</li><li>persistent project memory and an auditable trail</li><li>staying the author &mdash; where to rely on them, and where not to</li></ul><p class="lecture-takeaway">You leave with a workflow you can run the next day.</p></div>
</div>

The tools are genuinely useful today, and improving quickly — but long-horizon agents still drift, miss context, and need bounded tasks with external checks. The science stays mine: they change how carefully I can check it, not who is responsible for it.

<div class="contact-cta" markdown="0">
  <p>Happy to share the lecture or slides &mdash; or to bring a version to your group or department.</p>
  <a href="mailto:{{ site.author.email }}?subject=Using%20LLMs%20for%20research%20lecture">Get in touch</a>
</div>

</div>
