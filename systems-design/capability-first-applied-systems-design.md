##  ****Designing Responsible Human--AI Systems

### A practical method for building governable AI-enabled systems

Author

Jonathan Wong

CloudPedagogy

2026

DOI: https://doi.org/10.5281/zenodo.19009936

# Preface

Artificial intelligence is increasingly woven into the systems that
shape decisions, coordinate work, and monitor institutional activity.
Across sectors such as education, research, healthcare, government, and
industry, organisations are deploying AI-enabled tools to analyse
information, route requests, identify risks, and support complex
decision-making. These systems promise efficiency, scalability, and
insight at a scale previously impossible.

Yet something fundamental is often missing from the way these systems
are designed.

In many cases, AI-enabled systems are built by beginning with what
technology makes possible rather than with what human and institutional
capabilities must be preserved. Automation opportunities are identified,
models are trained, and workflows are redesigned to take advantage of
algorithmic outputs. Ethical guidance and governance frameworks may be
consulted, but they frequently appear as policy overlays rather than
structural constraints on system design.

The result is an increasingly common pattern: systems that appear
sophisticated and efficient on the surface but quietly erode the very
capabilities they were meant to support.

Professionals find themselves deferring to automated recommendations
they do not fully understand. Organisations struggle to explain how
certain outcomes occurred when systems behave in unexpected ways.
Governance bodies are asked to oversee systems whose architecture makes
meaningful oversight difficult or impossible. And individuals affected
by these systems often have limited ability to challenge or contest
decisions that appear to have emerged from opaque technical processes.

These failures rarely stem from malicious intent or careless
engineering. More often they arise because the systems were designed
without a clear method for ensuring that human judgement,
accountability, and institutional responsibility remain central once AI
becomes involved.

This book introduces **Capability-Driven Development (CDD)** as a
response to that gap.

Capability-Driven Development is a practical design method for building
AI-enabled systems in ways that preserve and strengthen human and
institutional capability. It provides a structured approach for ensuring
that decisions about automation, architecture, governance, and
evaluation are grounded in the capabilities that systems must support
rather than the technologies that systems might use.

At its core, Capability-Driven Development begins with a simple but
often overlooked principle:

Capability must precede automation.

Before designing a system that automates tasks, recommends actions, or
detects patterns, designers must first be able to answer a more
fundamental question: *What human and institutional capabilities must
remain intact when this system is introduced?*

These capabilities may include professional judgement, ethical
reasoning, accountability, contextual interpretation, or institutional
responsibility. In many domains---particularly those involving
education, public services, research, and governance---these
capabilities are not optional features of a system. They are the very
reason the system exists.

When automation is introduced without explicitly preserving these
capabilities, systems can unintentionally displace judgement, obscure
responsibility, and weaken the institutional practices they were meant
to support.

Capability-Driven Development therefore reverses a common design
pattern. Rather than beginning with technological possibility and later
asking how systems might be governed, CDD begins with capability
requirements and allows those requirements to constrain how systems are
designed.

This approach leads to systems where governance, accountability, and
ethical considerations are embedded directly into architecture,
workflow, and decision boundaries rather than imposed through external
policy or after-the-fact review.

The need for such an approach has become increasingly clear as
organisations attempt to reconcile the rapid adoption of AI technologies
with growing expectations for responsible and governable systems.
Current approaches to AI development often struggle to meet this
challenge for several reasons.

First, many development practices treat governance and accountability as
issues that arise after a system has been deployed. Ethical principles,
regulatory frameworks, and oversight mechanisms are introduced once
technical architectures have already been established. By that stage,
the architecture may limit the ability to introduce meaningful oversight
or contestation.

Second, existing development methods are typically designed to optimise
for technical performance, scalability, or efficiency. While these goals
are legitimate, they can inadvertently encourage system designs that
prioritise automation over judgement, throughput over care, and
optimisation over interpretability.

Third, governance discussions frequently occur at a level of abstraction
that makes them difficult to translate into system design decisions.
Principles such as fairness, transparency, or accountability are widely
endorsed, yet designers are rarely given practical guidance on how those
principles should shape workflows, architectures, and decision
boundaries.

Capability-Driven Development addresses these issues by providing a
design method that connects ethical reasoning, governance requirements,
and technical system design.

In doing so, it complements two other strands of work within the broader
CloudPedagogy ecosystem.

The first of these is the **AI Capability Framework**, which provides a
conceptual model for understanding what responsible and effective AI
capability looks like for individuals, teams, and institutions.
Organised across six domains---AI awareness, human--AI co-agency,
applied practice, ethics and impact, decision-making and governance, and
reflection and renewal---the framework helps organisations develop
shared language and insight about the capabilities required to work
responsibly with AI.

However, the AI Capability Framework deliberately remains
technology-agnostic. It does not prescribe how systems should be built,
nor does it dictate specific technical architectures or development
processes. Instead, it defines the capabilities that responsible AI use
should strengthen.

Capability-Driven Development builds upon that foundation by addressing
a different question: *How do we design systems that embody those
capabilities in practice?*

If the AI Capability Framework defines what capability is,
Capability-Driven Development defines how systems can be designed so
that capability is preserved rather than eroded.

The second related body of work is **Human--AI Governance Engineering**,
which explores how organisations can govern AI-enabled decision systems
at scale. That work focuses on institutional governance structures,
decision accountability, oversight mechanisms, and the broader societal
implications of intelligent systems embedded within organisational
infrastructure.

Capability-Driven Development sits between these two domains. It
provides the design method that translates capability principles and
governance expectations into the architecture and behaviour of specific
systems.

Together, these three elements form a coherent intellectual structure:

The AI Capability Framework defines the capabilities required for
responsible human--AI collaboration.

Capability-Driven Development provides the method for designing systems
that preserve and strengthen those capabilities.

Human--AI Governance Engineering addresses how organisations oversee,
regulate, and sustain those systems over time.

This book focuses specifically on the second of these: the design
method.

It explains how systems can be conceived, built, evaluated, and
ultimately retired in ways that keep human capability and institutional
responsibility at the centre of technological change.

The method presented here is not a software development methodology in
the conventional sense. It does not prescribe programming languages,
machine learning models, or development frameworks. Instead, it provides
a sequence of design considerations that ensure capability requirements
shape architectural and workflow decisions before automation becomes
embedded in system behaviour.

The chapters that follow introduce the conceptual foundations of
Capability-Driven Development, explain the method step by step, and
demonstrate its application through practical examples of AI-enabled
systems. These examples include decision support systems, workflow
orchestration systems, and monitoring and oversight systems---contexts
where the balance between automation and human responsibility is
particularly critical.

Throughout the book, the focus remains on a central question:

How can we design AI-enabled systems that strengthen human capability
rather than quietly replacing it?

This question is becoming increasingly urgent as organisations move from
experimenting with AI tools to embedding them within the infrastructure
of everyday work.

The goal of Capability-Driven Development is not to slow innovation or
prevent the use of automation where it is appropriate. Rather, it is to
ensure that innovation occurs in ways that remain explainable,
governable, and accountable as technologies evolve.

Responsible systems are not created simply by adopting ethical
guidelines or writing governance policies. They emerge when
responsibility, judgement, and oversight are designed directly into the
systems themselves.

Capability-Driven Development offers a practical way to do exactly that.

# PART I

# Why We Need Capability-Driven Development

# Chapter 1

# The Hidden Failure of AI System Design

Artificial intelligence systems are often evaluated according to the
wrong criteria.

When organisations assess AI-enabled systems, the conversation typically
focuses on questions such as:

- How accurate is the model?

- How quickly can the system process requests?

- How efficiently can workflows be automated?

- How much time or labour can be saved?

These questions are important, but they miss something far more
consequential. Many AI systems fail not because their models are
inaccurate, but because the systems surrounding those models quietly
undermine responsibility, judgement, and governance.

In other words, the most significant failures in AI systems are rarely
technical failures. They are failures of **system design**.

A model may produce useful insights. A classification algorithm may
perform well on benchmark tests. An orchestration tool may route
requests with impressive efficiency. Yet when these components are
embedded inside real organisational systems, the surrounding
architecture can create conditions where responsibility becomes unclear,
judgement becomes marginalised, and governance becomes ineffective.

These failures often remain hidden until something goes wrong.

When an unexpected outcome occurs---an unfair decision, an unexplainable
recommendation, or a harmful automated action---organisations frequently
struggle to answer a simple question:

Who is responsible for what happened?

At that point, the problem is no longer a technical one. It is a design
problem.

## The Illusion of Technical Success

Modern AI development culture tends to emphasise technical achievement.
Breakthroughs in machine learning, natural language processing, and
data-driven prediction have created an environment where technical
performance is often equated with system success.

However, the success of an AI model does not guarantee the success of an
AI-enabled system.

A system includes far more than the model that sits at its core. It
includes:

- the workflows through which outputs are used

- the interfaces through which humans interact with those outputs

- the governance structures that oversee system behaviour

- the decision boundaries that determine where authority lies

- the institutional responsibilities that persist regardless of
  automation

If these elements are poorly designed, even highly capable models can
produce systems that are fragile, opaque, or ethically problematic.

Consider a decision support system designed to assist professionals in
reviewing complex cases. The system may accurately summarise information
and highlight relevant factors. On paper, it appears to be a successful
application of AI.

Yet if the system's interface subtly encourages users to treat its
suggestions as authoritative conclusions, professional judgement may
begin to erode. Over time, decisions may become increasingly aligned
with the system's outputs, not because the system is always correct, but
because challenging it becomes inconvenient or socially discouraged.

In such a situation, the model has not failed. The system design has.

The technical component works exactly as intended, but the surrounding
system architecture has quietly shifted responsibility away from human
judgement toward automated guidance.

This phenomenon is far more common than many organisations realise.

## Automation Drift

One of the most persistent patterns in AI-enabled systems is what might
be called **automation drift**.

Automation drift occurs when systems that were originally designed to
assist humans gradually begin to shape or determine outcomes.

This drift rarely happens through a single explicit design decision.
Instead, it emerges gradually through a series of small changes.

A system that initially provides advisory information may later begin to
suggest preferred options. Those options may become default selections
within a workflow interface. Over time, users may find that deviating
from those defaults requires additional effort or justification.

Eventually, the system's outputs may become the de facto decision, even
though the formal design still describes the system as "decision
support."

At no point did anyone explicitly decide to automate the decision. Yet
in practice, the decision has been automated.

Automation drift is particularly difficult to detect because it often
appears as a natural evolution toward efficiency. Organisations may
interpret increased alignment with system outputs as evidence that the
system is performing well. After all, if people consistently follow the
system's suggestions, does that not indicate that the system is useful?

In reality, it may indicate that judgement is slowly being displaced.

Capability-Driven Development treats automation drift as a **design
failure**, not an inevitable side effect of technological progress.

Preventing automation drift requires systems that explicitly protect the
role of human judgement rather than assuming that it will remain intact
by default.

## Governance Gaps

Another hidden failure of many AI systems is the presence of
**governance gaps**.

Governance gaps arise when organisations attempt to oversee systems
whose design makes oversight difficult or ineffective.

In many institutions, governance is treated as something that occurs
outside the system itself. Policies are written, ethics committees are
formed, and guidelines are produced describing how AI should be used
responsibly.

These efforts are important, but they often operate independently from
the systems they are meant to govern.

When governance mechanisms are not embedded into system architecture,
they rely heavily on informal practices and individual judgement.
Oversight becomes reactive rather than proactive. Problems are
discovered after they occur rather than prevented through system design.

For example, a governance policy may state that decisions influenced by
AI should be explainable and reviewable. Yet if the system does not
record how recommendations were generated, who interacted with them, or
how final decisions were made, meaningful review becomes impossible.

Similarly, a policy may require that individuals affected by automated
systems be able to contest outcomes. But if the system's design does not
provide clear mechanisms for contestation or override, that right
remains theoretical rather than practical.

In such cases, governance has been declared but not implemented.

Capability-Driven Development addresses this problem by treating
governance as a **design property**. Systems must be built in ways that
allow accountability, oversight, and contestation to occur in practice,
not just in principle.

## Misplaced Trust in Algorithms

AI systems also introduce a subtle but powerful psychological effect:
**misplaced trust in algorithmic outputs**.

Humans often attribute a form of authority to computational systems.
Numbers, classifications, and rankings produced by algorithms can appear
objective or scientifically grounded, even when they are based on
uncertain or incomplete information.

This perception can lead to a phenomenon known as **automation bias**,
where people defer to algorithmic outputs even when their own judgement
suggests otherwise.

Automation bias does not necessarily arise because individuals believe
the system is infallible. Instead, it emerges because challenging the
system requires additional effort, confidence, or justification.

In organisational contexts, this dynamic can produce unintended
consequences. Professionals may begin to align their decisions with
algorithmic suggestions in order to avoid conflict, maintain
consistency, or comply with perceived expectations.

Over time, responsibility may gradually shift from human judgement to
algorithmic outputs.

The irony is that many systems were originally introduced to support
human decision-making, not replace it. Yet the structure of the system
makes deference to the algorithm the path of least resistance.

Preventing this dynamic requires system designs that actively reinforce
human authority rather than implicitly elevating algorithmic outputs.

## The Problem with "Human-in-the-Loop"

One of the most common responses to concerns about automation is the
concept of the **human-in-the-loop**.

The phrase is widely used to reassure stakeholders that humans remain
involved in AI-enabled processes. However, the concept is often far less
meaningful than it appears.

In many systems, humans are technically present within the process but
have little practical influence over outcomes.

For example, a workflow may require a human to approve a recommendation
generated by an AI system. Yet if the system presents the recommendation
as the default option, and if rejecting it requires additional
justification or effort, the human role becomes largely procedural.

The human is in the loop, but the loop itself has been designed to
favour automation.

In other cases, humans may be responsible for reviewing outputs without
having access to sufficient context to challenge them effectively. The
system may produce a classification or ranking without explaining how it
was generated or what uncertainties are involved.

Under these conditions, the human reviewer cannot meaningfully exercise
judgement.

Capability-Driven Development therefore treats vague references to human
oversight as insufficient. Human roles must be explicitly defined,
supported, and protected through system design.

Being "in the loop" is not enough. Humans must retain genuine authority
over outcomes.

## Capability Erosion

The patterns described above---automation drift, governance gaps,
misplaced trust in algorithms, and superficial human oversight---combine
to produce a deeper problem: **capability erosion**.

Capability erosion occurs when systems gradually weaken the human and
institutional abilities they were meant to support.

Professionals may lose opportunities to exercise judgement because
decisions are increasingly guided by automated suggestions.
Organisations may lose visibility into how outcomes are produced because
systems centralise information within opaque processes. Governance
bodies may lose the ability to intervene effectively because system
architectures limit oversight.

Over time, institutions may become dependent on systems whose behaviour
they do not fully understand and cannot easily modify.

Capability erosion rarely occurs suddenly. It emerges gradually through
small design decisions that prioritise efficiency, automation, or
optimisation without fully considering their impact on human capability.

Once these patterns become embedded in system architecture, they can be
difficult to reverse.

Capability-Driven Development was created to address this problem
directly.

Rather than asking how systems can automate tasks more effectively, it
asks a different question: how can systems be designed so that human and
institutional capability remains strong even as AI becomes embedded
within them?

This shift in perspective changes the entire design process.

Automation is no longer the starting point. Instead, designers begin by
identifying the capabilities that systems must support and protect.
These capabilities then shape decisions about human--AI boundaries,
governance mechanisms, architectural patterns, and evaluation practices.

The goal is not to reject automation, but to ensure that automation
operates within structures that preserve responsibility, judgement, and
institutional integrity.

The chapters that follow introduce Capability-Driven Development as a
practical method for achieving this goal.

By examining how systems can be designed to preserve capability rather
than erode it, we can begin to build AI-enabled systems that remain
accountable, governable, and trustworthy over time.

# Chapter 2

# The Governance Gap in Modern AI Systems

Artificial intelligence has advanced rapidly over the past decade.
Models have become more capable, datasets larger, and computing
infrastructure more powerful. As a result, organisations across sectors
are increasingly embedding AI into operational systems that influence
real decisions and outcomes.

At the same time, discussions about **AI governance** have grown
significantly. Governments publish regulatory guidance, institutions
adopt ethical principles, and professional bodies produce frameworks
intended to guide responsible AI use.

Despite this growing attention, a persistent problem remains.

Many organisations now possess **AI governance policies**, yet the
systems they deploy remain difficult to oversee, challenge, or explain.

This disconnect reveals a deeper issue: governance discussions often
occur separately from the design of the systems they are meant to
govern.

As a result, governance is declared in principle but rarely implemented
in practice.

This chapter explores why governance efforts frequently fail, how this
failure emerges from common development practices, and why meaningful
oversight requires a fundamentally different approach to system design.

## The Governance Paradox

Most organisations deploying AI today acknowledge the importance of
governance. Ethical principles such as fairness, transparency,
accountability, and responsibility are widely endorsed.

Yet when AI-enabled systems are examined closely, these principles often
have little direct influence on how systems actually operate.

This creates what might be called the **governance paradox**:

Organisations may express strong commitments to responsible AI while
deploying systems that are difficult to govern.

The paradox arises because governance is frequently treated as something
that exists **outside the system itself**.

Ethics committees review proposals. Compliance teams interpret
regulations. Policy documents describe acceptable practices. Training
sessions encourage responsible behaviour.

However, the systems that people interact with every day---the
interfaces, workflows, algorithms, and decision processes---may not
embody these principles in any meaningful way.

Governance therefore becomes a form of **institutional aspiration**
rather than a property of the system.

When problems occur, organisations discover that policies alone cannot
compensate for architectural decisions that make oversight impractical.

## Ethics Added After Deployment

One of the most common causes of governance failure is the timing of
ethical considerations.

In many AI projects, ethical questions are addressed **after** the
technical system has already been designed or deployed.

Development typically proceeds through a sequence that looks something
like this:

1.  Identify a process that could be automated or improved.

2.  Develop or integrate an AI model.

3.  Build the surrounding system architecture.

4.  Deploy the system to users.

5.  Conduct ethical review or governance assessment.

At this point, the fundamental structure of the system is already fixed.

Key design decisions have been made:

- where automation occurs

- how outputs are presented to users

- what information is logged

- what workflows exist

- how decisions are recorded

If ethical concerns arise during review, organisations often discover
that addressing them would require substantial redesign.

For example, reviewers may conclude that system outputs must be
explainable. Yet the model and data pipeline may not support meaningful
explanation.

Or they may determine that decisions influenced by AI must be auditable.
Yet the system may not record the information required to reconstruct
how recommendations were generated.

In these situations, ethical guidance becomes difficult to implement
because the system architecture was never designed to support it.

Ethics has been added **after the fact**, rather than shaping the system
from the beginning.

Capability-Driven Development treats this sequencing as a fundamental
design mistake.

Ethical and governance considerations must shape system structure from
the outset. Otherwise, governance becomes an external constraint applied
to systems that were never designed to accommodate it.

## Compliance Detached from System Design

A related problem occurs when governance is framed primarily in terms of
**compliance**.

Many organisations approach AI governance through regulatory or policy
compliance frameworks. They ask whether systems meet legal requirements,
adhere to guidelines, or satisfy institutional review processes.

Compliance is important. Regulations such as data protection laws,
sectoral guidelines, and emerging AI regulations establish necessary
safeguards.

However, compliance alone does not guarantee that systems are
governable.

A system may technically satisfy regulatory requirements while still
creating conditions that obscure responsibility or limit oversight.

For example, a system may comply with transparency regulations by
providing a written description of how its algorithm works. Yet if users
cannot see how specific outputs were generated in practice, that
transparency provides little practical value.

Similarly, a system may comply with fairness requirements by
demonstrating acceptable performance across demographic groups during
testing. Yet once deployed, the system may interact with organisational
processes in ways that produce unequal outcomes over time.

Compliance frameworks tend to focus on what must be documented or
demonstrated, not necessarily on how systems behave in real contexts.

When compliance is detached from system design, governance becomes an
administrative exercise rather than an operational capability.

Capability-Driven Development therefore treats compliance not as the
endpoint of governance, but as a **baseline requirement** that must be
supported by system architecture.

## Architecture Without Accountability

Perhaps the most significant governance challenge arises when technical
architecture is designed without explicit consideration of
accountability.

Architecture determines how information flows, how decisions are
recorded, and how people interact with systems. These structural choices
shape the conditions under which responsibility can be exercised or
examined.

Yet many AI systems are designed primarily around performance
considerations such as speed, scalability, or technical efficiency.

While these priorities are legitimate, they can unintentionally produce
architectures that make accountability difficult to maintain.

For instance, systems may integrate multiple models, data sources, and
automated components into complex pipelines. Outputs may be generated
through chains of processing steps that are not easily visible to users
or reviewers.

In such systems, tracing the origin of a specific outcome may require
navigating a technical structure that few people fully understand.

Responsibility therefore becomes diffuse.

When a problematic outcome occurs, responsibility may appear to lie
everywhere and nowhere at once: with the model developers, the system
architects, the data providers, the organisation deploying the system,
or the individual who relied on its output.

This ambiguity is not simply a legal issue. It is a design issue.

If systems are not structured to make decision pathways visible and
reviewable, accountability becomes extremely difficult to establish.

Capability-Driven Development addresses this challenge by treating
accountability as a **design constraint** rather than an organisational
aspiration.

Architectures must make it possible to see how outcomes emerge and who
is responsible for each stage of the process.

## The Limits of Policy-Based Governance

Another reason governance discussions often fail is the assumption that
**policy alone can regulate behaviour**.

Policies can define expectations, articulate values, and establish
rules. However, policies operate through human interpretation and
compliance.

When system behaviour is shaped by automated processes, relying solely
on policy can create gaps between intended practice and actual
operation.

Consider an organisational policy stating that professionals must
exercise independent judgement when using AI-assisted decision tools.

This policy may be entirely reasonable. Yet if the system interface
presents AI recommendations as default options, highlights them
visually, and requires additional effort to reject them, the system
itself subtly encourages alignment with those recommendations.

Under such conditions, policy and system design are working at cross
purposes.

People may technically retain the freedom to disagree with the system,
but the workflow structure makes doing so inconvenient or socially
discouraged.

Capability-Driven Development recognises that behaviour within systems
is shaped not only by policy but by **design choices**.

Responsible behaviour should be the **path of least resistance** within
the system, rather than something that requires deliberate effort to
maintain.

## Governance as an Engineering Problem

The patterns described above reveal a deeper insight: governance is not
merely an organisational or ethical issue.

It is also an engineering problem.

If governance is expected to function in practice, it must be supported
by system structures that make oversight, accountability, and
contestation possible.

This means governance cannot be treated as an external layer applied to
finished systems. It must be integrated into system design from the
beginning.

When governance is engineered into systems, several key properties
become possible:

- decision pathways can be reconstructed

- responsibilities are clearly located

- oversight bodies can review system behaviour meaningfully

- users can challenge outcomes when necessary

- systems can be adjusted without undermining accountability

In other words, governance becomes a **property of the system itself**.

This perspective aligns closely with the emerging discipline of
Human--AI Governance Engineering, which examines how organisations can
design decision systems that remain accountable and explainable even as
AI becomes embedded within them.

However, governance engineering alone does not specify how systems
should be designed to support these goals.

That is where Capability-Driven Development enters the picture.

## Bridging Governance and System Design

Capability-Driven Development provides the missing bridge between
governance principles and system architecture.

Rather than treating governance as a separate activity performed by
policy teams or oversight committees, CDD integrates governance
considerations directly into the design process.

The method begins by asking a fundamental question:

What capabilities must remain intact when AI becomes part of this
system?

These capabilities may include professional judgement, institutional
accountability, ethical reasoning, and the ability to explain or contest
decisions.

Once these capabilities are identified, they shape the design of the
system itself.

Human--AI boundaries define where authority resides.\
Ethical analysis identifies risks and constraints.\
Governance requirements determine what must be observable and
reviewable.\
Architecture ensures these constraints are structurally supported.

Through this process, governance is not added after deployment.

It is engineered into the system from the beginning.

## Why This Matters Now

The need for governance-aware system design is becoming increasingly
urgent.

AI is no longer confined to experimental tools or isolated decision
aids. It is being embedded into the infrastructure of organisations: the
systems that manage requests, evaluate applications, monitor
performance, and coordinate work.

As these systems become more central to institutional operations, the
consequences of poor governance design become more significant.

Organisations may find themselves unable to explain outcomes to
regulators, courts, or the public. Professionals may lose the ability to
exercise judgement effectively within automated workflows. Institutions
may become dependent on systems whose behaviour they cannot fully
oversee.

Addressing these risks requires moving beyond governance as policy and
toward governance as **system design**.

Capability-Driven Development provides a method for doing exactly that.

By aligning system architecture with capability requirements and
governance expectations, it enables organisations to build AI-enabled
systems that remain accountable, contestable, and trustworthy.

The next chapter introduces the conceptual foundation that makes this
approach possible: the idea that **capability must precede automation**.

# Chapter 3

# Capability as a Design Constraint

The previous chapters examined two persistent problems in modern AI
systems.

First, many systems fail not because their models are inaccurate, but
because responsibility and judgement become obscured within system
design. Automation drift, governance gaps, and superficial human
oversight can gradually erode the capabilities that institutions rely
upon.

Second, governance discussions frequently occur separately from the
design of the systems they are meant to regulate. Ethical principles and
compliance requirements are often articulated clearly, yet they remain
disconnected from the technical architectures that shape real system
behaviour.

These two problems are closely related.

When system design is driven primarily by technical opportunity or
efficiency goals, governance and capability become secondary
considerations. When governance is treated as an external layer applied
after systems are built, it struggles to influence the structures that
actually determine how decisions are made.

To resolve this tension, a different starting point is required.

Capability-Driven Development begins from a simple but powerful idea:

Capability should function as a design constraint.

Rather than asking how AI systems can automate tasks, the design process
begins by identifying the human and institutional capabilities that must
remain intact when automation is introduced. These capabilities then
shape decisions about architecture, workflows, and human--AI boundaries.

In this way, capability becomes the organising principle for system
design.

## What Do We Mean by Capability?

The word *capability* is often used in vague or aspirational ways.
Organisations may speak about building AI capability, digital
capability, or innovation capability without clearly defining what those
capabilities involve.

In the context of Capability-Driven Development, capability refers to
the ability of people and institutions to act responsibly, effectively,
and accountably within a system.

Capability is therefore not simply a technical property of a system. It
is a property of the **human--system relationship**.

A system strengthens capability when it enables people to exercise
judgement, understand outcomes, and take responsibility for decisions. A
system weakens capability when it obscures decision processes, displaces
judgement, or limits the ability of individuals and institutions to
intervene.

Understanding capability requires examining several interconnected
layers: human capability, professional capability, and institutional
capability.

## Human Capability

At its most fundamental level, capability refers to the capacities of
individuals.

Human capability includes the ability to:

- interpret information in context

- exercise judgement under uncertainty

- balance competing considerations

- recognise ethical implications

- explain and justify decisions

These capacities are central to many forms of professional practice.
Whether in medicine, education, law, research, or public administration,
individuals are expected to exercise judgement rather than simply follow
rules.

AI systems often promise to support these capabilities by providing
additional information, identifying patterns, or reducing cognitive
load. When designed well, such systems can indeed enhance human
decision-making.

However, when systems subtly shift authority toward automated outputs,
they can weaken these capabilities over time.

For example, if professionals repeatedly rely on automated
recommendations without critically examining them, opportunities to
develop judgement may diminish. If decision rationales are replaced by
algorithmic outputs, the ability to explain and defend decisions may
erode.

Capability-Driven Development therefore treats human capability as
something that must be **actively preserved through system design**.

Automation should support human judgement, not displace it.

## Professional Capability

Human capability is often expressed through professional roles.

Professionals operate within domains where expertise, training, and
ethical responsibility guide decision-making. Professional capability
therefore includes:

- specialised knowledge and expertise

- contextual interpretation of rules or policies

- ethical responsibility toward affected individuals

- the ability to justify decisions publicly or institutionally

AI systems can alter the conditions under which professional capability
operates.

When systems generate recommendations, prioritise cases, or surface risk
signals, professionals may increasingly work within decision
environments shaped by algorithmic outputs.

This is not inherently problematic. In many cases, AI can provide
valuable assistance by highlighting information that might otherwise be
overlooked.

The risk arises when systems gradually redefine the role of the
professional.

If algorithmic outputs become treated as authoritative conclusions,
professionals may shift from exercising judgement to validating
automated results. Instead of asking *what decision should be made*,
they may ask *whether the system's recommendation can be accepted*.

This subtle shift transforms the nature of professional responsibility.

Capability-Driven Development seeks to avoid this outcome by ensuring
that system design reinforces the role of professional judgement rather
than diminishing it.

## Institutional Capability

Capability also exists at the level of institutions.

Institutions such as universities, hospitals, public agencies, and
research organisations carry responsibilities that extend beyond
individual decisions. They must be able to:

- oversee decision processes

- demonstrate accountability to stakeholders

- review outcomes over time

- correct errors or unintended consequences

- maintain public trust

When AI systems are embedded within institutional workflows, these
capabilities can either be strengthened or weakened.

Systems that provide clear decision records, transparent workflows, and
structured oversight mechanisms can enhance institutional capability.
They allow organisations to understand how decisions were made and to
intervene when necessary.

Conversely, systems that centralise information within opaque technical
processes can weaken institutional capability. If outcomes emerge from
complex pipelines that are difficult to reconstruct or interpret,
oversight becomes challenging.

Institutions may find themselves responsible for decisions they cannot
fully explain.

Capability-Driven Development therefore treats institutional capability
as a core design consideration. Systems must support not only individual
decision-making but also institutional accountability.

## Professional Judgement as a Central Capability

Across human, professional, and institutional levels, one capability
repeatedly emerges as particularly important: **professional
judgement**.

Professional judgement involves interpreting information, weighing
competing considerations, and making decisions under conditions of
uncertainty.

Unlike automated decision rules, judgement cannot be fully reduced to
formal procedures. It requires context, experience, and ethical
reasoning.

In many domains, professional judgement serves as a safeguard against
rigid or overly mechanistic decision-making. It allows individuals to
recognise when rules or patterns do not adequately capture the
complexities of a particular situation.

When AI systems are introduced into such environments, preserving
professional judgement becomes essential.

If systems are designed in ways that implicitly prioritise algorithmic
outputs over human interpretation, professional capability may gradually
weaken. Decisions may become more consistent but less thoughtful, more
efficient but less accountable.

Capability-Driven Development treats professional judgement not as an
obstacle to automation but as a capability that must be preserved.

Systems should support judgement by providing relevant information and
analysis while leaving the final interpretation to human
decision-makers.

## The Relationship to the AI Capability Framework

The concept of capability used in Capability-Driven Development is
closely connected to the **AI Capability Framework**.

The AI Capability Framework provides a conceptual model for
understanding how individuals and institutions can work responsibly with
AI technologies. It identifies six interrelated domains of capability:

- AI awareness and orientation

- Human--AI co-agency

- Applied practice and innovation

- Ethics, equity, and impact

- Decision-making and governance

- Reflection, learning, and renewal

Together, these domains describe the capabilities required to engage
with AI systems thoughtfully and responsibly.

However, the AI Capability Framework focuses primarily on **people and
organisations** rather than system architecture. It asks what
capabilities professionals and institutions need in order to work
effectively with AI.

Capability-Driven Development addresses a complementary question:

How can systems be designed so that these capabilities are preserved and
strengthened?

In other words:

- The **AI Capability Framework** defines the capabilities that
  responsible AI use requires.

- **Capability-Driven Development** provides the design method for
  building systems that protect those capabilities.

This relationship is important. Without a clear understanding of
capability, system design risks drifting toward automation-driven
architectures. Without system design methods that respect capability,
even well-developed governance frameworks may struggle to influence
technological systems.

CDD therefore acts as the bridge between conceptual capability
frameworks and practical system design.

## Capability Before Automation

If capability is the organising principle of system design, a key
implication follows:

Automation decisions must be constrained by capability requirements.

This reverses the sequence commonly seen in technology development.

Instead of beginning with questions such as:

- What tasks can be automated?

- How can workflows be optimised?

- How can AI improve efficiency?

Capability-Driven Development begins with questions such as:

- What human capabilities must remain intact?

- What forms of judgement cannot be delegated to automation?

- What institutional responsibilities must remain visible and
  accountable?

Only after these questions are addressed do designers examine how AI
might support the system.

This shift may appear subtle, but it has significant implications for
system design. Automation becomes a **bounded tool** within a
capability-preserving architecture rather than the central organising
force of the system.

## Core Principles of Capability-Driven Development

From this perspective, several core principles emerge that guide
Capability-Driven Development.

### 1. Capability Precedes Automation

The primary principle of CDD is that capability requirements must be
identified before automation decisions are made.

Automation should be introduced only when it can support, rather than
undermine, human and institutional capability.

### 2. Responsibility Must Remain Visible

Systems should make it clear who is responsible for decisions and
outcomes.

Responsibility should not disappear into technical processes or become
distributed in ways that make accountability unclear.

### 3. Human Authority Must Be Structurally Preserved

Human judgement should not rely on informal practices or cultural
expectations alone.

System design should ensure that humans retain meaningful authority over
outcomes, including the ability to question, override, or reinterpret
automated outputs.

### 4. Governance Must Be Embedded in System Design

Oversight, traceability, and contestability should be supported by
system architecture.

Governance mechanisms should be built into workflows, data structures,
and decision processes rather than applied externally.

### 5. Systems Must Remain Contestable and Revisable

Responsible systems must allow outcomes to be questioned and revised.

Designs should support review, modification, and learning over time
rather than locking organisations into rigid technical structures.

### 6. Capability Should Strengthen Over Time

AI-enabled systems should contribute to organisational learning rather
than diminishing human expertise.

Systems should support reflection, feedback, and adaptation so that
capability grows rather than erodes.

## Capability as the Anchor of Responsible AI Systems

When capability functions as the organising principle of system design,
the relationship between humans and AI changes.

Instead of designing systems that gradually replace human roles,
organisations design systems that **support and stabilise human
capability**.

Automation becomes a tool within a broader architecture of
responsibility. Governance becomes a structural property of the system
rather than a separate oversight activity. Professional judgement
remains central even as AI contributes analytical or informational
support.

Capability-Driven Development therefore reframes the challenge of
responsible AI.

The question is no longer simply how to regulate AI technologies.

The question becomes:

How can we design systems where AI strengthens the capabilities that
individuals and institutions need in order to act responsibly?

The next chapter introduces the practical method that enables this
approach: the step-by-step structure of Capability-Driven Development.

# PART II

# The Capability-Driven Development Method

# Chapter 4

# Designing for Capability First

The previous chapter introduced capability as the organising principle
for responsible AI system design. If human judgement, professional
responsibility, and institutional accountability are to remain intact
when AI becomes embedded in systems, they cannot be treated as optional
considerations.

They must function as **design constraints**.

This chapter introduces the first practical step in Capability-Driven
Development: defining **capability intent**.

Capability intent establishes *why a system exists* in terms of the
capabilities it must support and protect. It ensures that system design
begins with responsibility, judgement, and institutional purpose rather
than technological opportunity.

Without this step, systems are easily pulled toward automation-first
thinking. With it, design decisions remain anchored in the capabilities
the system must preserve.

# Why System Design Must Start with Capability

Many technology projects begin with a familiar question:

What can we automate?

The motivation may be reasonable. Automation promises efficiency, speed,
and scalability. In many contexts it can reduce administrative burden or
surface information that would otherwise remain hidden.

However, starting with automation creates a subtle but powerful bias in
the design process.

Once automation becomes the organising goal, other considerations---such
as judgement, accountability, and governance---tend to be treated as
constraints that limit efficiency rather than as essential properties of
the system.

Design discussions may focus on:

- how much work can be automated

- how quickly cases can be processed

- how consistently decisions can be applied

- how much labour can be reduced

These priorities can easily overshadow deeper questions about
responsibility and capability.

Yet in many domains---particularly those involving education, public
services, research, healthcare, and governance---efficiency is not the
primary purpose of the system.

The primary purpose is often something more complex:

- enabling thoughtful decisions

- coordinating responsible action

- supporting professional judgement

- maintaining institutional accountability

If system design begins with automation, these capabilities may
gradually weaken.

Capability-Driven Development therefore reverses the usual sequence.

Instead of asking *what can be automated*, designers begin by asking:

What capabilities must this system strengthen or protect?

Only after this question is answered can responsible automation
decisions be made.

# What Is Capability Intent?

Capability intent defines the core purpose of a system in terms of
capability rather than technology.

It describes the capabilities that the system must support, preserve, or
strengthen once AI becomes part of it.

These capabilities may include:

- human judgement

- professional expertise

- institutional accountability

- transparency and explainability

- ethical responsibility

- the ability to contest or review outcomes

Capability intent therefore clarifies what the system must *not
undermine*.

It provides a reference point that guides every subsequent design
decision.

Without capability intent, systems drift toward whatever technical
configuration appears most efficient or convenient.

With capability intent, design choices can be evaluated against a clear
principle:

Does this decision strengthen or weaken the capability the system is
meant to support?

# Capability Intent as a Constraint

One of the most important characteristics of capability intent is that
it functions as a **constraint**.

In many development processes, goals are treated as flexible
aspirations. Designers may aim to support transparency or accountability
but allow those goals to be adjusted when technical challenges arise.

Capability intent operates differently.

Because it defines the purpose of the system, it establishes boundaries
that the system must respect.

For example, capability intent might specify that:

- final decisions must remain human

- professional judgement cannot be replaced by automated recommendations

- accountability for outcomes must remain visible

- decisions must be explainable and contestable

If later design proposals contradict these constraints---perhaps by
introducing automated decisions or opaque workflows---the design must be
reconsidered.

Capability intent therefore prevents the gradual erosion of
responsibility that often accompanies automation.

# The Risks of Capability Erosion

The need for capability intent becomes clearer when we examine how
systems unintentionally weaken capability over time.

Capability erosion rarely occurs through deliberate choices. Instead, it
emerges through small adjustments that appear reasonable individually
but collectively reshape the system.

These adjustments often occur during later development stages.

### Automation Expansion

A system initially designed to provide information may later be expanded
to provide recommendations. Recommendations may then become default
options in workflows.

Over time, users may increasingly accept these defaults, gradually
shifting authority toward the system.

### Efficiency Optimisation

Organisations may introduce changes to improve speed or consistency.
Decision steps may be removed or simplified in order to reduce delays.

While each change may appear beneficial, the cumulative effect may
reduce opportunities for judgement or review.

### Interface Framing

User interfaces can strongly influence behaviour.

If AI outputs are presented prominently while human reasoning fields
appear secondary, users may begin to treat system outputs as
authoritative.

### Institutional Dependence

As systems become integrated into everyday workflows, organisations may
grow dependent on them.

Replacing or modifying the system becomes increasingly difficult, even
when problems emerge.

Capability-Driven Development recognises that these risks are
structural.

They arise not because people behave irresponsibly but because system
design gradually shifts incentives and workflows.

Capability intent provides a way to detect and prevent these shifts
before they occur.

# Defining Capability Intent

Defining capability intent requires careful reflection about the
system's purpose.

Designers must ask several foundational questions:

### What capability does the system exist to support?

Is the system intended to strengthen professional judgement, coordinate
action, surface risks, or improve transparency?

The answer should be framed in terms of human or institutional
capability rather than technical function.

### What capabilities must not be displaced?

Certain capabilities may be considered non-negotiable.

For example:

- final decisions must remain human

- ethical judgement must not be delegated to automation

- institutional responsibility cannot be outsourced to algorithms

These constraints should be stated explicitly.

### What outcomes would indicate capability erosion?

Designers should also consider how the system might weaken capability.

For example:

- professionals deferring uncritically to system outputs

- responsibility becoming unclear when errors occur

- oversight bodies unable to review decisions

Identifying these risks early helps guide later design choices.

# Introducing the System Capability Brief

In Capability-Driven Development, capability intent is captured in a
document known as the **System Capability Brief**.

The System Capability Brief serves as the foundation for the entire
design process.

It provides a structured description of:

- the system's purpose in capability terms

- the capabilities the system must strengthen

- the constraints the system must respect

- the risks of capability erosion

This document functions as a reference point throughout development.

Whenever new features, automation opportunities, or architectural
changes are proposed, they can be evaluated against the System
Capability Brief.

If a proposal undermines the defined capability intent, it should be
reconsidered.

# What the System Capability Brief Contains

While the exact format may vary, a System Capability Brief typically
includes several key elements.

### System Context

A short description of the organisational context in which the system
will operate.

This includes the kinds of decisions, actions, or workflows the system
will influence.

### Capability Purpose

A clear statement describing the capability the system exists to
support.

For example:

- supporting consistent professional decision-making

- coordinating responsible action across teams

- surfacing signals that require oversight

- strengthening institutional transparency

This section focuses on capability rather than technology.

### Non-Negotiable Constraints

Explicit statements describing capabilities that must remain intact.

Examples might include:

- final decisions remain human

- professional discretion must be preserved

- oversight mechanisms must remain practical

- accountability for outcomes must remain visible

These constraints shape later design decisions.

### Capability Risks

Identification of potential risks that could erode capability.

For example:

- automation drift

- algorithmic authority replacing judgement

- reduced transparency in decision pathways

- increased dependence on opaque technical processes

Acknowledging these risks helps guide later design steps.

# Why the System Capability Brief Matters

The System Capability Brief plays a crucial role in the design process.

First, it provides **clarity of purpose**.

Technology projects often accumulate features and objectives over time.
Without a clear articulation of purpose, it becomes difficult to
evaluate whether new features support or undermine the system's goals.

Second, it provides a shared reference point.

System design often involves multiple stakeholders: developers, domain
experts, governance bodies, and organisational leaders.

The capability brief ensures that all participants share a common
understanding of what the system is meant to achieve.

Third, it provides a safeguard against drift.

As systems evolve, new features or optimisations may appear attractive.
The capability brief allows designers to evaluate these changes against
the system's original purpose.

If a proposed change threatens capability intent, the design can be
reconsidered before it becomes embedded in architecture.

# Capability Intent in Practice

Defining capability intent does not eliminate complexity from system
design. Instead, it makes that complexity visible.

Designers may discover that certain automation opportunities conflict
with capability constraints. They may find that achieving efficiency
requires careful balancing with accountability.

These tensions are not signs of failure.

They are signs that the design process is taking responsibility
seriously.

Capability-Driven Development does not attempt to eliminate trade-offs.
Instead, it ensures that trade-offs are **explicit and deliberate**.

When automation decisions are made, they are made with a clear
understanding of how they affect capability.

# The First Step in Capability-Driven Development

Capability intent therefore forms the first step in the
Capability-Driven Development method.

Before system architecture is defined, before models are selected, and
before workflows are optimised, designers must clearly articulate:

What capability does this system exist to support?

The answer becomes the foundation for every subsequent step.

Once capability intent is defined, the next task is to determine how
responsibilities should be distributed between humans and AI systems.

The next chapter introduces the second step of Capability-Driven
Development: defining **human--AI boundaries**.

# Chapter 5

# Defining Human--AI Boundaries

Once capability intent has been defined, the next step in
Capability-Driven Development is to determine **how responsibility will
be distributed between humans and AI systems**.

This step is often overlooked in technology design. In many AI-enabled
systems, the relationship between human judgement and automated
processes remains implicit. Systems are described as providing
"assistance," "decision support," or "automation," yet the actual
boundaries between human and machine authority are rarely defined
clearly.

The consequences of this ambiguity can be significant.

When boundaries are unclear, responsibility becomes difficult to locate.
Automated outputs may gradually be treated as decisions. Humans may
remain nominally responsible for outcomes while lacking meaningful
authority over how those outcomes are produced.

Capability-Driven Development addresses this risk by requiring that
**human--AI boundaries be designed explicitly**.

These boundaries define who does what, when, and under what conditions
within a system. They determine where authority resides, how delegation
occurs, and how humans can intervene when automated processes produce
uncertain or problematic results.

In short, human--AI boundaries determine how responsibility is enacted
in practice.

# Why Human--AI Boundaries Must Be Explicit

Many organisations assume that human oversight exists simply because
people remain involved somewhere in the workflow.

For example, a system may generate recommendations that a human must
approve before action is taken. From a governance perspective, this may
appear sufficient: a human remains "in the loop."

However, such arrangements often fail to preserve meaningful human
authority.

In practice, several patterns frequently emerge.

Users may feel pressure to align with automated recommendations because
rejecting them requires additional effort or explanation. Interfaces may
present system outputs as default options, subtly encouraging
acceptance. Over time, human reviewers may begin to treat automated
outputs as authoritative conclusions rather than suggestions.

The human role remains present, but its influence diminishes.

This problem arises because the boundaries between human and AI roles
were never clearly defined.

Capability-Driven Development therefore treats implicit boundaries as a
**design failure**.

If systems influence decisions, the roles of humans and AI must be
deliberately specified.

# What Human--AI Boundaries Define

Human--AI boundaries describe the **division of roles, responsibilities,
and authority** within a system.

They clarify several essential aspects of system behaviour.

First, they define **where AI may assist**.

AI systems may analyse data, summarise information, detect patterns, or
generate possible options. These forms of assistance can enhance human
capability by reducing cognitive load or highlighting relevant
considerations.

Second, boundaries define **where humans must decide**.

Certain decisions require interpretation, ethical judgement, or
contextual understanding that cannot be delegated safely to automated
systems. These decision points must remain under human authority.

Third, boundaries identify where automation is prohibited.

In some contexts---particularly those involving rights, safety, or
institutional responsibility---automation may introduce unacceptable
risks. Explicit boundaries prevent systems from drifting toward
automated outcomes.

Fourth, boundaries define how escalation and intervention occur.

When automated processes encounter uncertainty, conflict, or unusual
cases, the system must provide clear pathways for human involvement.

Finally, boundaries specify how humans can override automated outputs.

Human decision-makers must be able to challenge system behaviour when it
appears inappropriate or incorrect.

Together, these elements define the operational relationship between
humans and AI systems.

# Authority: Who Has the Final Say?

One of the most important boundary questions concerns **authority**.

Authority determines who has the final right to decide outcomes within
the system.

In many domains, the answer should be clear: responsibility for outcomes
remains human.

For example, in systems supporting professional decision-making, AI may
provide analysis or recommendations. However, the authority to interpret
information and determine outcomes should remain with human
professionals.

When authority is ambiguous, systems can drift toward automated
decision-making even when this was not the original intention.

Authority should therefore be explicitly defined.

Designers must answer questions such as:

- Who has final decision authority?

- Under what conditions can automated processes act independently?

- When must human approval always be required?

These questions ensure that responsibility remains visible and
enforceable.

# Delegation: What Can AI Do?

Once authority is defined, designers must consider **delegation**.

Delegation concerns the tasks that can appropriately be assigned to AI
systems.

AI systems are well suited to tasks such as:

- analysing large datasets

- identifying patterns or anomalies

- summarising complex information

- generating possible options or scenarios

Delegating such tasks can significantly enhance human capability by
reducing cognitive burden.

However, delegation should not be confused with decision-making
authority.

Delegation means that AI systems perform specific tasks within clearly
defined boundaries. Humans retain responsibility for interpreting
results and determining outcomes.

Capability-Driven Development therefore distinguishes between
**assistance** and **delegation**.

Assistance provides information or insight. Delegation assigns tasks.
Neither should replace human authority over decisions.

# Escalation: When Humans Must Intervene

No automated system can anticipate every possible situation.

Unexpected cases, ambiguous inputs, or conflicting signals may arise
that require human judgement.

For this reason, systems must include clear **escalation mechanisms**.

Escalation defines the conditions under which cases are referred to
human decision-makers.

Examples might include:

- uncertain or conflicting system outputs

- cases that fall outside expected patterns

- decisions involving high ethical or legal risk

- signals indicating potential harm or bias

Without clear escalation pathways, systems may continue operating under
conditions where automation is no longer appropriate.

Escalation mechanisms ensure that human judgement can re-enter the
process when needed.

# Override: Preserving Human Authority

Even when systems function correctly, situations may arise where
automated outputs appear inappropriate or incomplete.

Human decision-makers must therefore be able to **override** system
behaviour.

Override mechanisms allow humans to:

- reject automated recommendations

- adjust system classifications or prioritisation

- intervene in workflows

- correct errors or unintended outcomes

Equally important is the ability to **record overrides**.

Recording when and why humans disagree with system outputs provides
valuable information for governance and system improvement.

Override mechanisms reinforce the principle that AI outputs remain
advisory rather than authoritative.

# Why "Human-in-the-Loop" Is Not Enough

The phrase "human-in-the-loop" is often used to describe responsible AI
systems.

However, the phrase can be misleading.

A human may technically remain involved in a process while having little
real influence over outcomes.

For example, a workflow may require a human to confirm system-generated
decisions. If rejecting those decisions requires justification or
additional work, users may gradually treat confirmation as a routine
formality.

In such cases, the human role becomes procedural rather than
substantive.

Capability-Driven Development therefore treats the presence of humans
within a system as insufficient.

The critical question is not whether humans are present, but **whether
they retain meaningful authority**.

Meaningful authority requires:

- clear decision rights

- the ability to challenge automated outputs

- access to information necessary for judgement

- workflows that support rather than discourage intervention

Without these conditions, "human-in-the-loop" systems can easily become
automated decision systems in practice.

# Common Boundary Failure Modes

Several common failures arise when human--AI boundaries are not designed
explicitly.

### Implicit Authority

Systems may present outputs in ways that imply authority even when they
are intended to be advisory.

### Rubber-Stamping

Human approval steps may become routine confirmations rather than
genuine decision points.

### Hidden Automation

Automation may occur within system processes without users fully
understanding its influence on outcomes.

### Inaccessible Overrides

Systems may technically allow overrides but make them difficult to
perform or justify.

### Escalation Avoidance

Escalation mechanisms may exist but remain unused because they are
cumbersome or poorly integrated into workflows.

These failures demonstrate why boundaries must be explicitly designed
and documented.

# Introducing the Human--AI Boundary Map

In Capability-Driven Development, human--AI boundaries are captured in a
design artefact known as the **Human--AI Boundary Map**.

The Human--AI Boundary Map provides a structured representation of how
responsibility is distributed across the system.

It typically identifies:

- decision points within workflows

- the actors responsible for each decision

- the role of AI at each stage

- escalation triggers and pathways

- override mechanisms and authority

This map helps designers visualise how humans and AI interact throughout
the system.

It also provides a reference point for governance discussions and system
evaluation.

# Why the Boundary Map Matters

The Human--AI Boundary Map serves several important purposes.

First, it makes responsibility **visible**.

Rather than assuming that human oversight exists, the map shows exactly
where human authority operates within the system.

Second, it prevents **automation drift**.

If future design changes threaten to shift authority toward automation,
the map provides a reference against which those changes can be
evaluated.

Third, it supports governance and oversight.

Governance bodies can use the boundary map to understand where decisions
occur and how responsibility is distributed.

Finally, it supports **system design**.

Architectural decisions---such as workflow structure, logging
mechanisms, and user interfaces---can be aligned with the defined
boundaries.

# Boundaries as the Foundation of Responsible Systems

Human--AI boundaries transform abstract principles into operational
design.

They ensure that:

- assistance does not become substitution

- efficiency does not override accountability

- automation remains bounded and governable

Without explicit boundaries, systems gradually evolve in ways that may
weaken human capability.

With clear boundaries, systems can support human judgement while
benefiting from AI assistance.

Capability-Driven Development therefore treats boundary design as a
central step in building responsible AI systems.

Once capability intent and human--AI boundaries are defined, the next
task is to examine the **ethical, equity, and risk implications** of
those boundaries.

The next chapter explores how Capability-Driven Development addresses
these considerations as core design inputs rather than post-deployment
concerns.

# Chapter 6

# Designing for Ethics, Equity, and Risk

Once capability intent has been established and human--AI boundaries
have been defined, the next step in Capability-Driven Development is to
examine the **ethical, equity, and risk implications** of the system.

This step is frequently misunderstood in AI development.

In many technology projects, ethics is treated as a set of high-level
principles or guidelines. These principles may appear in policy
documents, codes of conduct, or governance frameworks. They often
include widely accepted values such as fairness, transparency,
accountability, and respect for human rights.

While these principles are important, they often remain disconnected
from the way systems are actually designed and implemented.

Capability-Driven Development approaches ethics differently.

Rather than treating ethics as an abstract discussion or a compliance
exercise, CDD treats **ethical and risk considerations as design
inputs**. Ethical analysis is not something that happens after a system
has been built. It is something that shapes how the system is built in
the first place.

This chapter examines how designers can identify foreseeable harms,
understand how risks are distributed, anticipate misuse, and assess
potential equity impacts. It also introduces the **Risk and Misuse
Register**, a design artefact that helps teams document and address
these issues systematically.

# Ethics as a Design Input

In many AI initiatives, ethical concerns emerge late in the development
process.

A system may be designed and implemented with the goal of improving
efficiency or enabling new capabilities. Only once the system is
operational do organisations begin to ask whether it introduces unfair
outcomes, undesirable incentives, or unexpected harms.

At that stage, addressing ethical issues can be extremely difficult.

Architectural decisions may already constrain what can be changed.
Workflows may have become dependent on system behaviour. Organisations
may have invested heavily in infrastructure that is difficult to
redesign.

For this reason, Capability-Driven Development treats ethics not as a
retrospective evaluation but as a **forward-looking design activity**.

The key question becomes:

What harms could reasonably arise from the use or misuse of this system?

This question encourages designers to examine potential consequences
before system behaviour becomes embedded in organisational practice.

# Foreseeable Harm

One of the most important tasks in ethical design is identifying
**foreseeable harm**.

Foreseeable harm does not refer to hypothetical or extreme scenarios.
Instead, it refers to outcomes that could plausibly occur given the
system's design, context, and patterns of use.

Examples of foreseeable harm may include:

- incorrect or misleading recommendations influencing decisions

- automated classifications that disadvantage certain groups

- delayed escalation of urgent cases due to algorithmic prioritisation

- users relying too heavily on system outputs without critical review

These harms may arise even when the system functions technically as
intended.

For example, a model might accurately detect patterns in historical
data. Yet if that data reflects historical inequities, the system may
reproduce those inequities in its outputs.

Similarly, a workflow system designed to optimise case routing may
inadvertently make certain types of cases less visible, delaying
appropriate attention.

Identifying foreseeable harm requires thinking beyond technical
performance. It requires examining how the system interacts with human
behaviour, organisational incentives, and real-world contexts.

Capability-Driven Development encourages teams to explore these
possibilities early in the design process.

# Understanding Risk Distribution

Another critical consideration is **risk distribution**.

Risk distribution refers to who bears the consequences when systems fail
or behave unexpectedly.

In many AI systems, risks are not distributed evenly.

For example:

- individuals affected by automated decisions may experience the
  consequences of errors

- frontline professionals may be expected to manage system outputs
  without having influence over system design

- institutions may carry legal or reputational responsibility for
  outcomes produced by complex technical systems

Understanding where risk sits is essential for responsible system
design.

A system that shifts risk onto individuals without giving them
meaningful recourse or explanation is ethically problematic. Similarly,
systems that require professionals to assume responsibility for outcomes
they cannot influence create governance challenges.

Capability-Driven Development therefore encourages designers to ask:

- Who bears the consequences if the system is wrong?

- Who has the authority to intervene when problems occur?

- Are some groups exposed to risk without adequate protection?

Answering these questions can reveal structural inequities that might
otherwise remain hidden.

# Misuse and System Drift

Another important dimension of risk involves **misuse**.

Systems are rarely used exactly as designers intended. Over time, they
may be repurposed, extended, or interpreted in ways that differ from
their original purpose.

For example, a decision-support tool might gradually be used as a
decision-making tool. A monitoring system designed to surface risks
might be used to evaluate individual performance. A workflow system
intended to coordinate work might become a mechanism for enforcing
compliance.

These shifts can occur gradually and unintentionally.

Organisational pressures---such as efficiency targets, performance
metrics, or resource constraints---may encourage people to use systems
in ways that were not anticipated during design.

Capability-Driven Development therefore encourages teams to ask:

- How might this system be misused or repurposed?

- What pressures might encourage inappropriate reliance on automation?

- How could system scope gradually expand beyond its intended purpose?

Anticipating misuse allows designers to introduce safeguards that limit
these risks.

For example, systems may include explicit scope boundaries, transparency
mechanisms, or governance review processes that prevent misuse from
becoming normalised.

# Equity Impacts

Ethical design must also consider **equity impacts**.

AI systems often operate within social and institutional contexts where
inequalities already exist. If these inequalities are not considered
during system design, technology may inadvertently reinforce them.

Equity impacts may arise in several ways.

### Differential Access

Some users may have greater ability to understand or navigate system
outputs. Systems that assume certain levels of technical literacy or
institutional knowledge may disadvantage others.

### Unequal Outcomes

Systems trained on historical data may reflect patterns that
disadvantage certain groups. Even when models are technically accurate,
their outputs may perpetuate inequities embedded in past decisions.

### Burden Shifting

Certain roles or groups may absorb disproportionate workload or
responsibility when systems are introduced. For example, frontline staff
may be required to resolve complex cases generated by automated systems
without additional support.

Capability-Driven Development encourages teams to examine these
possibilities early.

Questions that help reveal equity impacts include:

- Who benefits most from the system?

- Who may be disadvantaged by its operation?

- Are certain groups exposed to greater scrutiny or burden?

- Does the system assume access or capacity that cannot be guaranteed?

Equity analysis does not eliminate all inequalities, but it helps ensure
that designers understand how systems interact with existing social
structures.

# Introducing the Risk and Misuse Register

To ensure that ethical and risk considerations are documented and
addressed systematically, Capability-Driven Development introduces a
design artefact known as the **Risk and Misuse Register**.

The Risk and Misuse Register records the ethical, equity, and
operational risks identified during system design.

Rather than treating risk analysis as an informal discussion, the
register provides a structured way to capture potential issues and track
how they are addressed.

Typically, the register includes several elements.

### Risk Description

A clear description of the potential harm or misuse scenario.

### Affected Parties

Identification of the individuals or groups who may be affected.

### Likelihood and Severity

An assessment of how likely the risk is to occur and how significant its
consequences could be.

### Mitigation Strategies

Design changes, safeguards, or governance mechanisms intended to reduce
or manage the risk.

### Residual Risk

Recognition that some risks cannot be eliminated entirely and must be
managed through oversight or governance.

# Why the Risk and Misuse Register Matters

The Risk and Misuse Register serves several important purposes.

First, it encourages **explicit reflection** about potential harms.
Rather than assuming that systems will be used responsibly, designers
examine how they might fail or be misused.

Second, it provides **transparency for governance bodies**. Oversight
committees or institutional leaders can review identified risks and
evaluate whether mitigation strategies are adequate.

Third, it supports **accountability over time**. If problems emerge
after deployment, the register provides a record of what risks were
anticipated and how they were addressed.

Finally, it ensures that ethical considerations influence **system
design decisions**.

If a particular risk cannot be mitigated effectively, designers may need
to revisit earlier steps such as capability intent or human--AI
boundaries.

# Ethical Design as Ongoing Responsibility

Addressing ethics, equity, and risk during system design does not
eliminate the need for ongoing governance.

Systems operate within dynamic environments where organisational
practices, social contexts, and technological capabilities continue to
evolve.

New risks may emerge as systems interact with real-world workflows.
Patterns of use may change in ways that designers did not anticipate.

For this reason, ethical analysis should not be treated as a one-time
activity.

Instead, it should form part of a broader process of **continuous review
and learning**.

Capability-Driven Development therefore integrates ethical analysis with
later steps such as governance design, evaluation, monitoring, and
system iteration.

By identifying risks early and revisiting them over time, organisations
can ensure that AI-enabled systems remain aligned with their ethical and
institutional responsibilities.

# Ethics as a Structural Property of Systems

Ultimately, the goal of this step is not simply to identify ethical
concerns.

The goal is to ensure that systems are designed in ways that make
ethical behaviour structurally supported.

When ethical considerations shape human--AI boundaries, workflows, and
governance mechanisms, responsible behaviour becomes easier to maintain.

Conversely, when ethics is treated as an abstract principle disconnected
from system design, it becomes difficult to enforce in practice.

Capability-Driven Development therefore treats ethics, equity, and risk
as core elements of system architecture.

By examining foreseeable harm, understanding risk distribution,
anticipating misuse, and evaluating equity impacts, designers can build
systems that are not only technically effective but also socially
responsible.

The next chapter examines how these ethical and risk considerations
translate into concrete mechanisms for **governance and oversight**.

# Chapter 7

# Engineering Governance Into Systems

In many organisations, governance is treated as something that exists
outside technological systems.

Policies are written. Ethical guidelines are drafted. Oversight
committees are established. Compliance requirements are defined. These
governance mechanisms are intended to ensure that technology is used
responsibly and that organisations remain accountable for the systems
they deploy.

However, when artificial intelligence systems are introduced, governance
often encounters a practical problem: **the system itself was not
designed to support governance**.

The architecture of the system may not record how decisions were
produced. Interfaces may not reveal the reasoning behind automated
recommendations. Workflows may not allow decisions to be challenged or
reviewed effectively. Logs may capture technical events but fail to
record the human and institutional decisions that shaped outcomes.

Under these conditions, governance becomes largely symbolic.

Policies may exist, but the system makes it difficult to enforce them.
Oversight committees may exist, but they lack the information required
to evaluate system behaviour. Organisations remain responsible for
outcomes, but they lack the mechanisms needed to demonstrate
accountability.

Capability-Driven Development addresses this problem by treating
governance not as a policy layer but as a **system design requirement**.

If systems influence decisions, governance must be engineered directly
into the architecture of those systems.

This chapter explains how that can be achieved by focusing on four
essential governance properties:

- accountability

- auditability

- contestability

- scope control

Together, these properties ensure that AI-enabled systems remain
explainable, governable, and aligned with institutional responsibility.

To operationalise these ideas, Capability-Driven Development introduces
a key design artefact: the **Governance and Oversight Plan**.

# Governance as a Structural Feature of Systems

The introduction of AI into organisational systems changes the nature of
governance.

Traditional governance approaches often assume that human actors perform
decisions in visible and accountable ways. When individuals exercise
judgement, responsibility can be traced through organisational
structures.

AI-enabled systems complicate this relationship.

Automated processes may influence decisions in ways that are difficult
to observe. Recommendations may shape outcomes even when humans formally
retain decision authority. Complex workflows may obscure how information
flows through the system.

If governance mechanisms rely solely on external oversight---such as
policy reviews or periodic audits---they may fail to capture how the
system actually operates in practice.

For governance to function effectively, systems must be designed in ways
that make responsibility visible and traceable.

This is the central premise of governance engineering.

Rather than asking how governance bodies can monitor systems from the
outside, Capability-Driven Development asks a different question:

How can systems be designed so that governance becomes an inherent
property of their operation?

Answering this question requires attention to several key design
principles.

# Accountability

The first and most fundamental governance property is
**accountability**.

Accountability ensures that responsibility for system outcomes can be
clearly identified.

In many AI systems, accountability becomes blurred because decisions
emerge from interactions between multiple components: data sources,
algorithms, automated workflows, and human actions.

Without careful design, this complexity can make it difficult to
determine who is responsible for particular outcomes.

For example, if a system generates a recommendation that influences a
professional decision, responsibility might be distributed across
several actors:

- the designers who created the system

- the organisation that deployed it

- the professionals who relied on its outputs

- the data sources that shaped the model's behaviour

If accountability is not clearly defined, organisations may struggle to
explain how decisions were made.

Capability-Driven Development addresses this by ensuring that system
design supports **clear lines of responsibility**.

Accountability mechanisms may include:

- identifying responsible actors at each decision point

- recording when automated outputs influence decisions

- documenting when human judgement overrides system recommendations

- defining institutional responsibility for system outcomes

These mechanisms ensure that responsibility does not disappear inside
complex technical systems.

# Auditability

Closely related to accountability is **auditability**.

Auditability refers to the ability to examine how a system produced a
particular outcome.

This does not necessarily require that every algorithm be fully
interpretable. Instead, it requires that systems record sufficient
information to reconstruct decision pathways.

An auditable system should be able to answer questions such as:

- What information did the system use?

- What outputs did the system generate?

- How were those outputs used within workflows?

- Who reviewed or acted on them?

Without such records, organisations cannot effectively evaluate system
behaviour.

Auditability is particularly important when systems operate at scale.
When hundreds or thousands of decisions are influenced by automated
processes, occasional errors or unexpected outcomes are inevitable.

If those outcomes cannot be investigated, organisations lose the ability
to learn from mistakes or improve system design.

Capability-Driven Development therefore encourages designers to
integrate auditability into system architecture through mechanisms such
as:

- decision logs that record key system outputs

- workflow records documenting human interactions with system outputs

- metadata describing model versions and data sources

- event histories capturing escalation or override actions

These records allow organisations to trace how decisions unfolded over
time.

# Contestability

Governance also requires the ability to **challenge system outcomes**.

This property is known as **contestability**.

Contestability ensures that individuals affected by system outputs---or
professionals responsible for interpreting those outputs---can question
or appeal decisions when necessary.

In many AI systems, contestability is limited because the system's
architecture does not support meaningful challenge.

For example, if a system produces a classification or risk score without
revealing how it was generated, individuals may have little basis for
questioning the outcome. Similarly, if workflows lack mechanisms for
reviewing or revising decisions, contestation becomes impractical.

Capability-Driven Development treats contestability as a design
requirement.

Systems should provide mechanisms that allow users to:

- request clarification about system outputs

- challenge or override automated recommendations

- escalate contested outcomes for human review

- document disagreements with system behaviour

These mechanisms ensure that system outputs remain subject to human
judgement rather than becoming unquestioned authority.

Contestability is particularly important in contexts where system
outputs affect individuals' rights, opportunities, or wellbeing.

# Scope Control

Another critical governance property is **scope control**.

Scope control refers to mechanisms that prevent systems from gradually
expanding beyond their intended purpose.

Technological systems often evolve over time. New features are added.
Workflows are extended. Data sources are integrated. While these changes
may appear incremental, they can significantly alter how systems
influence decisions.

For example, a system initially designed to support case triage might
gradually begin influencing prioritisation decisions. A monitoring
system might expand into performance evaluation. A recommendation system
might begin shaping policy decisions.

These changes may occur without deliberate governance review.

Scope control ensures that such expansions do not occur unnoticed.

Capability-Driven Development encourages teams to define the **intended
scope** of a system clearly and to implement mechanisms that detect when
the system begins to operate beyond that scope.

These mechanisms may include:

- explicit documentation of system purpose

- governance review triggers when system functionality changes

- monitoring indicators that detect shifts in system use

- architectural constraints limiting certain types of automation

Scope control protects institutions from gradual shifts that could
undermine capability, accountability, or ethical alignment.

# Introducing the Governance and Oversight Plan

To integrate these governance properties into system design,
Capability-Driven Development introduces the **Governance and Oversight
Plan**.

The Governance and Oversight Plan is a structured document that
describes how governance will operate within and around the system.

Rather than existing as a generic policy statement, the plan connects
governance mechanisms directly to system architecture and workflows.

Typically, the Governance and Oversight Plan addresses several key
questions.

### Accountability Structure

Who is responsible for system behaviour, oversight, and maintenance?

### Audit Mechanisms

What information will the system record to support review and
investigation?

### Contestation Pathways

How can system outputs be challenged or reviewed?

### Scope Boundaries

What functions and decisions fall within the system's intended scope?

### Oversight Roles

Which individuals or bodies are responsible for reviewing system
performance?

# Why the Governance and Oversight Plan Matters

The Governance and Oversight Plan serves several important purposes.

First, it aligns governance with system architecture.

Rather than treating governance as an external constraint, the plan
ensures that governance mechanisms are supported by system design.

Second, it provides clarity for stakeholders.

Developers, operators, governance bodies, and end users can understand
how responsibility is distributed and how oversight operates.

Third, it supports institutional accountability.

If questions arise about system behaviour, organisations can demonstrate
that governance mechanisms were designed intentionally rather than added
as an afterthought.

Finally, it enables continuous improvement.

By documenting governance structures and review processes, organisations
can refine them over time as systems evolve.

# Governance as an Engineering Discipline

The integration of governance into system architecture represents a
significant shift in how organisations approach AI-enabled systems.

Traditionally, governance has been treated as a managerial or regulatory
function. Engineers build systems, and governance bodies oversee them.

Capability-Driven Development suggests that this separation is no longer
sufficient.

When AI systems influence decisions, governance must be considered part
of the system itself.

This does not mean that engineers replace governance professionals.
Rather, it means that system designers must collaborate closely with
governance stakeholders to ensure that systems support accountability,
transparency, and oversight.

In this sense, governance becomes a design challenge as well as a policy
challenge.

# From Governance Principles to Operational Systems

By embedding accountability, auditability, contestability, and scope
control into system architecture, organisations can move from abstract
governance principles to operational governance practices.

Policies and ethical commitments become enforceable because the system
itself supports them.

This approach also strengthens institutional capability.

When governance mechanisms are engineered into systems, organisations
retain the ability to understand, challenge, and adapt the technologies
they deploy.

Without such mechanisms, organisations risk becoming dependent on
systems whose behaviour they cannot fully examine or control.

Capability-Driven Development therefore treats governance engineering as
a central step in responsible AI system design.

With governance structures in place, the next challenge is ensuring that
systems continue to perform as intended over time.

The next chapter examines how Capability-Driven Development supports
**evaluation, monitoring, and learning** once systems are deployed.

# Chapter 8

# Architecture as Responsibility

System architecture is often treated as a technical concern.

When organisations design AI-enabled systems, architectural discussions
typically focus on issues such as performance, scalability, reliability,
and integration. Engineers consider how components communicate, how data
flows through the system, and how models interact with infrastructure.

These technical considerations are important, but they obscure a deeper
reality:

Architecture is not neutral.

The structure of a system determines how authority is exercised, how
decisions unfold, and how responsibility is distributed. Architectural
choices shape who can intervene, who can observe system behaviour, and
who ultimately controls outcomes.

In other words, architecture encodes values.

Capability-Driven Development treats architecture not merely as a
technical structure but as an expression of **institutional
responsibility**. The way systems are designed determines whether
governance, accountability, and human judgement can function effectively
once AI becomes embedded within organisational workflows.

This chapter examines how architecture shapes responsibility, how design
decisions influence authority and oversight, and how specific
architectural patterns can support responsible human--AI collaboration.

# Architecture Encodes Values

Every system architecture reflects assumptions about how work should
occur.

These assumptions may not be explicitly stated, but they are embedded in
system structure.

For example, a system that automatically routes cases based on
algorithmic classification assumes that the algorithm should influence
prioritisation. A system that requires human confirmation before action
assumes that humans must retain final authority. A system that logs
every interaction assumes that traceability and oversight are important.

These choices reveal underlying values about responsibility,
transparency, and control.

In many AI projects, architectural decisions are made primarily for
reasons of efficiency or convenience. Engineers optimise workflows to
minimise latency, reduce manual steps, or automate repetitive tasks.

However, when systems influence decisions, architectural optimisation
must also consider governance implications.

A workflow that eliminates human review may improve efficiency but
remove an important safeguard. A system that hides intermediate
calculations may simplify interfaces but reduce transparency. A design
that centralises control within a model may increase automation but
weaken institutional oversight.

Capability-Driven Development therefore encourages designers to
recognise that **architecture expresses ethical and governance
choices**, not just technical ones.

# Architecture Shapes Authority

One of the most important ways architecture influences systems is
through the distribution of authority.

Authority is not determined solely by policy statements or
organisational roles. It is shaped by the pathways through which
information and decisions flow.

For example, consider a system where an algorithm generates a
recommendation that is automatically inserted into a workflow interface
as the default option.

Even if policy states that the human reviewer retains decision
authority, the architecture encourages alignment with the automated
recommendation. The default option becomes the easiest path.

Over time, users may come to treat the recommendation as the effective
decision.

Conversely, an architecture that requires active interpretation---such
as presenting system outputs alongside alternative perspectives---may
reinforce human judgement.

In this way, architecture influences behaviour.

Authority is not only about who formally decides. It is also about how
systems make decisions easier or harder.

Capability-Driven Development therefore emphasises architectural designs
that preserve meaningful human authority.

# Architecture Determines Oversight

Architecture also determines whether oversight is possible.

Oversight requires visibility into system behaviour. Governance bodies
must be able to understand how decisions occur and how automated
processes influence outcomes.

If a system's architecture hides intermediate steps or fails to record
key interactions, oversight becomes difficult.

For example, a system that generates automated outputs without logging
the underlying inputs or model versions prevents meaningful review. When
unexpected outcomes occur, investigators cannot determine how the result
was produced.

Similarly, if workflows do not record when humans override system
recommendations, organisations lose valuable insight into how system
outputs interact with professional judgement.

Capability-Driven Development therefore treats oversight as an
architectural property.

Systems must be designed to support visibility, traceability, and
review.

This includes:

- recording decision pathways

- logging interactions between humans and system outputs

- maintaining histories of model behaviour and updates

- capturing escalation and override events

These features allow organisations to observe system behaviour and
evaluate whether it aligns with institutional expectations.

# Architecture and Responsibility Distribution

Architectural choices also determine how responsibility is distributed
across systems.

In some designs, responsibility becomes highly centralised.

For example, a system that relies heavily on automated decision engines
may concentrate authority within algorithmic components. Human actors
may simply execute system outputs.

In other designs, responsibility may remain distributed across multiple
actors. AI components provide information or analysis, but humans retain
interpretive authority.

Capability-Driven Development favours architectures that support
responsibility distribution rather than responsibility displacement.

This means designing systems where AI assists human capability rather
than replacing it.

Achieving this balance requires careful attention to workflow structure,
system interfaces, and decision boundaries.

Architecture must ensure that human actors remain meaningfully involved
in the processes that determine outcomes.

# Key Architectural Design Patterns

Capability-Driven Development introduces several architectural patterns
that help preserve capability and governance within AI-enabled systems.

These patterns provide reusable structures that align technical design
with responsibility and oversight.

While specific implementations may vary across domains, the patterns
illustrate how architecture can support responsible system behaviour.

# Pattern 1: Decision Support Architecture

In a **decision support architecture**, AI systems provide analysis,
recommendations, or insights, but human actors retain decision
authority.

The architecture separates analysis from decision-making.

AI components may generate summaries, predictions, or classifications.
These outputs are presented to human decision-makers alongside relevant
contextual information.

Importantly, the system does not automatically convert recommendations
into actions.

Human actors interpret the outputs and determine outcomes.

This pattern preserves professional judgement while allowing AI systems
to enhance information processing.

# Pattern 2: Assisted Workflow Architecture

In an **assisted workflow architecture**, AI systems help coordinate
processes without determining final outcomes.

For example, a system might prioritise cases for review, identify
anomalies within data streams, or suggest potential responses.

However, each step in the workflow includes explicit human interaction
points.

These interaction points allow humans to review, interpret, and adjust
system outputs.

The architecture therefore supports efficiency without eliminating human
oversight.

# Pattern 3: Escalation Architecture

Some systems operate largely through automated processes but include
mechanisms for human intervention when necessary.

In an **escalation architecture**, the system identifies situations
where automated behaviour may be insufficient.

Examples might include:

- uncertainty in model outputs

- conflicting signals within data

- detection of potential harm or bias

When such conditions arise, the system escalates the case to human
review.

This pattern allows systems to operate efficiently under normal
conditions while ensuring that complex or ambiguous cases receive human
attention.

# Pattern 4: Transparent Logging Architecture

Transparency is essential for governance and learning.

A **transparent logging architecture** ensures that key system
interactions are recorded and available for review.

These logs may include:

- system inputs and outputs

- human interactions with system recommendations

- escalation events

- override decisions

Such records allow organisations to reconstruct how decisions unfolded.

They also provide valuable data for evaluating system performance and
identifying areas for improvement.

# Pattern 5: Modular Responsibility Architecture

Complex systems often involve multiple components, including data
pipelines, models, workflow engines, and interfaces.

In a **modular responsibility architecture**, these components are
designed so that responsibilities remain visible and separable.

For example:

- models generate predictions but do not control workflow execution

- workflow systems manage processes but do not interpret predictions

- human actors retain authority over final decisions

This separation prevents any single component from quietly absorbing
excessive authority.

It also makes systems easier to audit and modify.

# Architecture and Capability Preservation

The architectural patterns described above share a common goal:
**preserving human and institutional capability**.

When architecture reinforces human authority, supports oversight, and
records system behaviour, organisations retain the ability to govern
their technological systems.

Conversely, architectures that prioritise automation without these
safeguards may gradually erode capability.

Human judgement becomes marginalised, oversight becomes difficult, and
responsibility becomes difficult to trace.

Capability-Driven Development therefore treats architecture as a
critical site where responsibility is enacted.

# From Technical Systems to Responsible Systems

Ultimately, the architecture of a system determines whether governance
principles can function in practice.

Policies may emphasise accountability, transparency, and fairness. Yet
if system architecture does not support these properties, those
principles remain aspirational rather than operational.

By recognising architecture as a form of responsibility, organisations
can design systems that remain aligned with institutional values even as
AI technologies evolve.

Capability-Driven Development therefore encourages designers to ask not
only how systems should function technically, but also how they should
function **institutionally and ethically**.

When architecture reflects these considerations, systems become more
than technical tools.

They become infrastructures that support responsible human--AI
collaboration.

The next chapter examines how such systems can be evaluated and
monitored over time to ensure that capability, governance, and
responsibility remain intact as systems evolve.

# Chapter 9

# Evaluating Human--AI Systems

Once an AI-enabled system has been designed and deployed, a new
challenge emerges: **how should the system be evaluated over time?**

In many technology projects, evaluation focuses primarily on technical
performance. Teams measure metrics such as accuracy, latency,
throughput, or system uptime. These indicators are important because
they help ensure that systems operate reliably and efficiently.

However, when AI systems influence decisions, performance metrics alone
are insufficient.

A model may perform well on benchmark tests yet still undermine
professional judgement. A workflow may process cases efficiently while
quietly disadvantaging certain groups. A recommendation system may
generate accurate predictions while shifting authority away from human
decision-makers.

In other words, technical performance does not necessarily indicate
responsible system behaviour.

Capability-Driven Development therefore expands the scope of system
evaluation.

Instead of evaluating only technical outputs, organisations must also
examine how systems affect human capability, institutional practices,
and governance structures.

This chapter explores how evaluation can address these broader concerns
by focusing on three areas:

- capability outcomes

- behavioural indicators

- governance review

Together, these dimensions allow organisations to assess whether AI
systems remain aligned with their intended purpose.

# The Limits of Performance Metrics

Modern AI development culture places strong emphasis on performance
metrics.

Machine learning models are evaluated according to measures such as
accuracy, precision, recall, and F1 scores. System engineers examine
metrics such as response time, throughput, and reliability.

These indicators are useful for understanding how technical components
behave.

However, they reveal very little about how systems influence human
decision-making and institutional behaviour.

Consider a system that predicts which cases should be prioritised for
review. The model may achieve high predictive accuracy when evaluated
against historical data.

Yet if professionals begin to treat system outputs as definitive
priorities, important contextual information may be overlooked. The
system may inadvertently shape behaviour in ways that undermine
professional judgement.

From a technical perspective, the system performs well.

From an institutional perspective, the system may be introducing new
risks.

Performance metrics cannot capture these dynamics because they measure
outputs rather than **effects on human capability and governance**.

Capability-Driven Development therefore emphasises evaluation approaches
that examine how systems influence real-world practices.

# Evaluating Capability Outcomes

The first dimension of evaluation focuses on **capability outcomes**.

Capability outcomes describe how a system affects the abilities of
individuals and institutions to exercise judgement, responsibility, and
oversight.

When systems are introduced into organisational workflows, they can
influence capability in several ways.

Some systems strengthen capability by improving access to information or
reducing cognitive burden. Others may weaken capability by encouraging
excessive reliance on automated outputs.

Evaluating capability outcomes requires examining whether the system
supports or undermines key capabilities identified during the design
phase.

Questions that may guide this evaluation include:

- Do professionals feel more informed or less confident when using the
  system?

- Does the system support thoughtful decision-making or encourage rapid
  acceptance of automated outputs?

- Are professionals able to challenge system recommendations
  effectively?

- Do governance bodies retain visibility into how decisions occur?

Capability outcomes are not always captured through numerical metrics.

They often require qualitative insight into how systems shape human
behaviour and organisational practices.

Methods such as interviews, user feedback, and observational studies can
help reveal whether systems strengthen or erode capability.

# Behavioural Indicators

A second important dimension of evaluation involves **behavioural
indicators**.

Behavioural indicators examine how people actually interact with the
system.

Even when system design aims to preserve human authority, real-world use
may evolve in unexpected ways. Professionals may begin to rely heavily
on automated outputs, or they may bypass system recommendations
entirely.

Observing behavioural patterns can reveal whether the system is
functioning as intended.

Examples of behavioural indicators may include:

- the frequency with which system recommendations are accepted or
  rejected

- how often human overrides occur

- whether escalation mechanisms are used appropriately

- patterns of reliance on automated classifications or rankings

These indicators help reveal the **practical influence of the system**.

For example, if overrides never occur, this could indicate one of two
things:

- the system is extremely accurate, or

- users feel unable or discouraged from challenging it

Similarly, if escalation mechanisms are rarely used, it may indicate
that users do not recognise when escalation is necessary or that the
process is difficult to access.

Behavioural indicators therefore provide insight into how system design
interacts with human behaviour.

# Governance Review

The third dimension of evaluation focuses on **governance review**.

Governance review examines whether oversight structures continue to
function effectively once the system is deployed.

Even well-designed systems can drift over time. Organisational practices
may change, system functionality may expand, or new forms of risk may
emerge.

Regular governance review ensures that systems remain aligned with
institutional expectations.

Key questions for governance review may include:

- Are governance roles and responsibilities still appropriate?

- Do oversight bodies receive sufficient information to evaluate system
  behaviour?

- Are risk mitigation strategies working as intended?

- Have new risks emerged since deployment?

Governance review may involve multiple stakeholders, including system
designers, governance committees, domain experts, and frontline
professionals.

By examining system behaviour from multiple perspectives, organisations
can identify issues that might otherwise remain hidden.

# Monitoring System Drift

Evaluation is not a one-time activity.

Once systems are deployed, their behaviour may evolve through several
forms of **system drift**.

### Behavioural Drift

Users may begin interacting with the system in ways that differ from
original expectations.

### Organisational Drift

Institutional practices may adapt around system behaviour, changing how
decisions are made.

### Technical Drift

Models may perform differently as data distributions change over time.

Monitoring these forms of drift is essential for maintaining system
integrity.

Capability-Driven Development therefore encourages organisations to
establish monitoring processes that track both technical performance and
human interaction patterns.

# Signals of Capability Erosion

One of the most important goals of evaluation is detecting **capability
erosion**.

Capability erosion occurs when systems gradually weaken the human or
institutional abilities they were meant to support.

Early warning signs may include:

- professionals becoming reluctant to challenge system outputs

- decision processes becoming overly dependent on automated
  recommendations

- governance bodies losing visibility into system behaviour

- increasing difficulty explaining how outcomes are produced

When such signals appear, organisations may need to revisit system
design.

Possible responses could include redesigning interfaces, strengthening
escalation mechanisms, or adjusting human--AI boundaries.

Evaluation therefore plays a crucial role in maintaining system
responsibility over time.

# Integrating Evaluation Into System Design

Effective evaluation does not begin after system deployment.

Instead, evaluation should be considered during the design phase.

Designers should ask questions such as:

- What indicators will reveal whether the system strengthens capability?

- What behavioural signals should be monitored?

- What information will governance bodies require?

By answering these questions early, organisations can ensure that
systems collect the data needed for meaningful evaluation.

For example, logging mechanisms introduced during system design can
capture interactions between users and system outputs. These records can
later support behavioural analysis and governance review.

In this way, evaluation becomes part of the system's architecture rather
than an external assessment process.

# Evaluation as Institutional Learning

Ultimately, evaluation should not be viewed as a compliance exercise.

Its purpose is not simply to confirm that systems meet predefined
standards.

Instead, evaluation should support **institutional learning**.

AI systems operate within complex and evolving environments. No design
process can anticipate every possible outcome or interaction.

Evaluation allows organisations to observe how systems behave in
practice, learn from experience, and refine their approaches.

When evaluation processes are integrated with governance and system
monitoring, organisations can adapt their systems in ways that preserve
capability and responsibility.

# Beyond Performance

The key insight of Capability-Driven Development is that the success of
AI systems cannot be judged by performance metrics alone.

Responsible systems must also support human capability, maintain
institutional accountability, and remain open to governance oversight.

By examining capability outcomes, behavioural indicators, and governance
processes, organisations can gain a more complete understanding of how
systems function in practice.

This broader approach to evaluation ensures that AI-enabled systems
remain aligned with the values and responsibilities that motivated their
creation.

The next chapter explores how systems can evolve responsibly over time
through **iteration, adaptation, and continuous improvement**.

# Chapter 10

# Iteration Without Drift

No system remains static.

Once AI-enabled systems are deployed into real organisational
environments, they inevitably evolve. New features are requested. Models
are updated. Workflows are refined. Data sources change. Users adapt
their practices around the system.

Iteration is therefore a normal and necessary part of system life.

However, when AI systems influence decisions, iteration introduces a
subtle but significant risk: **systems can gradually drift away from
their original purpose**.

Changes that appear small or technically reasonable may alter how
authority is distributed, how decisions are made, or how oversight
operates. Over time, these incremental adjustments can transform a
system in ways that undermine the very capabilities it was meant to
support.

Capability-Driven Development therefore emphasises the importance of
**iteration without drift**.

Systems must be able to evolve, but that evolution must remain aligned
with the capability intent, human--AI boundaries, and governance
structures defined during the design phase.

This chapter explores how organisations can support responsible system
evolution while avoiding automation creep and preserving institutional
accountability.

# Why System Evolution Is Inevitable

Once a system enters operational use, it becomes embedded in a dynamic
environment.

Several forces drive system evolution.

### Operational Learning

Users quickly discover practical improvements that designers did not
anticipate. They may request changes to interfaces, workflows, or system
outputs to better support their work.

### Technical Updates

Machine learning models may require retraining as data patterns evolve.
Infrastructure components may be upgraded. Security vulnerabilities may
require architectural adjustments.

### Organisational Change

Institutions themselves evolve. Policies change, priorities shift, and
new regulatory requirements emerge. Systems must adapt to remain aligned
with organisational goals.

### Expanded Expectations

Successful systems often attract additional uses. Stakeholders may
request that the system perform new functions or support new forms of
decision-making.

These forms of evolution are not inherently problematic. In many cases,
they are signs that a system is becoming more useful and integrated into
organisational workflows.

However, without careful oversight, evolution can gradually reshape the
system in unintended ways.

# The Risk of Automation Creep

One of the most common risks associated with system evolution is
**automation creep**.

Automation creep occurs when systems gradually shift from assisting
human judgement to replacing it.

This shift rarely occurs through a single deliberate decision. Instead,
it emerges through a sequence of small changes.

For example:

- A system initially provides recommendations.

- Later, those recommendations become default selections within a
  workflow.

- Over time, the system begins automatically applying those
  recommendations unless users intervene.

Each individual change may appear reasonable.

Yet together they may transform the system from a decision-support tool
into an automated decision system.

Automation creep often occurs because incremental improvements focus on
efficiency rather than capability preservation.

Designers may aim to reduce friction within workflows or minimise manual
steps. While these goals can improve productivity, they can also weaken
the role of human judgement.

Capability-Driven Development treats automation creep as a **governance
concern rather than a purely technical issue**.

Preventing automation creep requires mechanisms that ensure system
changes remain aligned with the original capability intent.

# Recognising Capability Drift

Automation creep is one form of a broader phenomenon known as
**capability drift**.

Capability drift occurs when system changes gradually alter how human
capability functions within the system.

Early warning signs of capability drift may include:

- decreasing frequency of human overrides

- declining use of escalation pathways

- increased reliance on automated outputs without contextual
  interpretation

- governance bodies losing visibility into system behaviour

These signals suggest that the relationship between humans and AI may be
shifting in ways that were not originally intended.

Monitoring such indicators allows organisations to intervene before
drift becomes embedded in system architecture.

# Responsible System Evolution

Capability-Driven Development approaches system iteration through the
principle of **responsible system evolution**.

Responsible evolution means that system changes are evaluated not only
for their technical benefits but also for their impact on capability,
governance, and accountability.

Whenever a significant system modification is proposed, designers should
revisit several key questions.

### Does the change affect capability intent?

If the system begins performing new functions, the capabilities it
supports may change.

### Does the change alter human--AI boundaries?

Automation changes may shift authority or reduce opportunities for human
judgement.

### Does the change affect governance mechanisms?

New features may require additional oversight or logging mechanisms.

### Does the change introduce new risks?

Modifications may create unforeseen ethical, operational, or security
concerns.

By examining system changes through these lenses, organisations can
ensure that iteration remains aligned with responsible design
principles.

# Documenting Change

A central requirement for responsible iteration is **documenting system
changes clearly**.

In many technology projects, change documentation focuses on technical
updates such as software versions, bug fixes, or performance
improvements.

While these records are important, they rarely capture how system
changes influence decision processes or governance structures.

Capability-Driven Development encourages teams to maintain documentation
that records **how system behaviour evolves over time**.

This documentation may include:

- descriptions of new features or capabilities

- changes to human--AI boundaries

- updates to governance mechanisms

- modifications to risk mitigation strategies

Documenting these changes ensures that organisations retain a historical
record of how the system has evolved.

Such records are valuable for governance review, evaluation, and future
system redesign.

# Change Logs and System History

One practical mechanism for documenting system evolution is the **system
change log**.

A system change log records significant modifications to system
architecture, models, workflows, or governance mechanisms.

Each entry may include:

- a description of the change

- the rationale for the modification

- the expected impact on system behaviour

- any governance review associated with the change

Maintaining a change log allows organisations to trace how the system
has developed over time.

If unexpected outcomes occur, investigators can examine whether recent
modifications may have contributed to the issue.

This transparency strengthens institutional accountability.

# Governance Review of System Changes

In systems that influence important decisions, significant modifications
should be subject to **governance review**.

Governance review does not necessarily require complex approval
processes for every minor change.

However, modifications that affect system scope, decision authority, or
risk exposure should be evaluated by appropriate oversight bodies.

Examples of changes that may require governance review include:

- introducing automated actions that previously required human approval

- expanding the system's use into new domains

- integrating new data sources that affect decision outcomes

- altering escalation or override mechanisms

Governance review ensures that system evolution remains aligned with
institutional responsibilities.

# Iteration as a Learning Process

Responsible system evolution is not only about preventing drift.

It is also an opportunity for **organisational learning**.

As systems operate in real environments, organisations gain insight into
how AI interacts with human behaviour, institutional processes, and
external contexts.

These insights can inform improvements to system design.

For example:

- behavioural indicators may reveal where users need better interpretive
  support

- evaluation findings may highlight opportunities to strengthen
  governance mechanisms

- risk monitoring may reveal emerging ethical or operational concerns

Iteration allows organisations to refine systems so that they better
support capability and responsibility.

# Maintaining Alignment With Capability Intent

Throughout the life of a system, the original **capability intent**
remains a critical reference point.

Capability intent describes the capabilities that the system was
designed to support and preserve.

During system evolution, teams should periodically revisit this intent
and ask:

- Does the system still support these capabilities?

- Have new features shifted the balance between automation and
  judgement?

- Are governance mechanisms still adequate for current system behaviour?

If the system begins to diverge from its original intent, organisations
may need to reconsider how the system should evolve.

Sometimes this may require redesigning components of the system. In
other cases, it may involve clarifying governance structures or
revisiting human--AI boundaries.

# Designing Systems That Can Evolve Responsibly

The goal of Capability-Driven Development is not to prevent change.

Technological systems must evolve to remain useful.

Instead, the goal is to ensure that change occurs intentionally rather
than accidentally.

By documenting modifications, monitoring capability indicators, and
reviewing significant changes through governance processes,
organisations can guide system evolution responsibly.

Systems remain adaptable without losing sight of the principles that
shaped their design.

# Iteration as Stewardship

Ultimately, the evolution of AI-enabled systems should be understood as
a form of **institutional stewardship**.

Organisations that deploy such systems are responsible not only for
their initial design but also for how they evolve over time.

Without careful stewardship, systems may drift toward greater
automation, reduced transparency, and diminished human authority.

With responsible iteration, systems can continue to support human
capability while adapting to new challenges and opportunities.

Capability-Driven Development therefore treats iteration as an ongoing
responsibility rather than a purely technical process.

The final chapter explores how systems can eventually reach the end of
their lifecycle and how organisations can retire or replace them
responsibly.

# Chapter 11

# Designing for System Endings

Technological systems are often designed with growth and expansion in
mind.

Organisations invest significant effort into developing new systems,
deploying them at scale, and integrating them into everyday workflows.
Once a system becomes embedded in institutional practice, attention
typically shifts toward improving performance, expanding functionality,
and supporting ongoing use.

Yet an important reality is frequently overlooked:

All systems eventually reach an end.

Technologies become outdated. Organisational priorities change.
Regulatory environments evolve. Data sources shift. New tools emerge
that replace older ones. In some cases, systems may simply prove
inadequate for the needs they were designed to address.

Despite this inevitability, many systems are never explicitly designed
with endings in mind.

Instead, they persist long after their original purpose has faded.
Legacy systems remain embedded in institutional infrastructure,
difficult to modify and even harder to retire. Responsibilities become
entangled with outdated technologies, making change risky and
disruptive.

For AI-enabled systems---particularly those that influence
decisions---this problem becomes even more significant.

When such systems are retired or replaced without careful planning,
organisations risk losing accountability records, institutional
knowledge, and governance mechanisms. Decisions previously influenced by
automated processes may become difficult to reconstruct. Lessons learned
from system operation may disappear.

Capability-Driven Development therefore introduces an important
principle:

Responsible systems must be designed with endings in mind.

Designing for system endings ensures that organisations can retire or
replace systems without losing responsibility, oversight, or
institutional learning.

This chapter explores how organisations can plan for responsible system
retirement, capture lessons from system use, and manage transitions
between technologies.

# Why Systems Persist Beyond Their Purpose

Many organisations struggle to retire systems once they have become
embedded in operational workflows.

Several factors contribute to this persistence.

### Institutional Dependence

Over time, systems become integrated into organisational processes.
Staff rely on them to complete routine tasks. Data flows through their
infrastructure. Removing the system may appear disruptive or risky.

### Loss of System Knowledge

As systems age, the individuals who originally designed or implemented
them may move on. Institutional knowledge about how the system operates
may diminish, making it difficult to modify or replace.

### Governance Uncertainty

When systems influence decisions, organisations may worry about losing
the records or oversight mechanisms associated with those systems.

### Incremental Adaptation

Rather than replacing outdated systems, organisations often modify them
incrementally. New features are added to legacy infrastructure,
gradually increasing complexity.

These dynamics can lead to systems remaining operational long after they
should have been replaced.

Capability-Driven Development encourages organisations to recognise that
system endings are not failures. They are a normal and necessary part of
responsible technological stewardship.

# Responsible System Retirement

Responsible system retirement involves deliberately managing the end of
a system's operational life.

Rather than simply switching a system off or replacing it abruptly,
organisations should consider how retirement affects accountability,
governance, and institutional knowledge.

Several questions should guide retirement planning.

### What responsibilities does the system currently support?

Before retiring a system, organisations must understand how it
influences decisions and workflows. Responsibilities embedded in the
system may need to be transferred to new processes or technologies.

### What records must be preserved?

AI-enabled systems often generate logs, decision histories, and
governance records. These records may be essential for accountability,
auditing, or regulatory compliance.

### What dependencies exist?

Other systems, workflows, or organisational practices may depend on the
retiring system. These dependencies must be identified and addressed
before retirement occurs.

### How will stakeholders adapt?

Professionals who rely on the system may require training or support to
transition to alternative tools or workflows.

Responsible retirement therefore requires planning, documentation, and
communication.

# Institutional Learning

One of the most valuable aspects of system retirement is the opportunity
for **institutional learning**.

Over the course of its operational life, a system generates significant
knowledge about how AI interacts with human decision-making and
organisational processes.

This knowledge should not disappear when the system is retired.

Instead, organisations should capture lessons learned from system
operation.

These lessons may include:

- insights into how users interacted with system outputs

- observations about how automation influenced behaviour

- governance challenges encountered during system use

- improvements that could inform future system design

Documenting such insights allows organisations to refine their
approaches to AI system development.

Capability-Driven Development therefore encourages teams to treat system
retirement as an opportunity to reflect on what worked well and what
could be improved.

# Transition Planning

When systems are retired, organisations must also manage the
**transition to new processes or technologies**.

Transitions can be complex because systems often play multiple roles
within institutional workflows.

For example, an AI-enabled decision-support system may:

- provide analytical insights

- structure workflow processes

- record decision histories

- support governance review

Replacing such a system may require introducing several new components
or redesigning workflows entirely.

Transition planning helps ensure that these changes occur smoothly.

Key aspects of transition planning include:

### Capability Preservation

The capabilities supported by the retiring system must be maintained or
strengthened in the replacement system.

### Governance Continuity

Oversight mechanisms should continue to function during and after the
transition.

### Data and Record Migration

Important records and logs should be preserved and transferred where
appropriate.

### Stakeholder Communication

Users must understand why the system is being retired and how new
processes will function.

Without careful transition planning, organisations risk disrupting
workflows or weakening governance structures.

# Avoiding Institutional Amnesia

One of the greatest risks associated with system retirement is
**institutional amnesia**.

When systems disappear without preserving their operational history,
organisations lose valuable insights about how those systems functioned.

This loss can have several consequences.

Governance bodies may struggle to investigate past decisions. Designers
of future systems may repeat mistakes that were previously identified.
Organisations may lose evidence demonstrating how decisions were made.

Capability-Driven Development therefore encourages organisations to
treat system history as an important institutional asset.

Preserving system documentation, decision logs, and evaluation findings
ensures that knowledge gained during system operation remains available
for future learning.

# Retirement as Responsible Stewardship

Designing systems with endings in mind reflects a broader philosophy of
responsible technological stewardship.

Organisations that deploy AI systems influence not only operational
processes but also institutional culture and decision-making practices.

Responsible stewardship requires recognising that technologies evolve
and that systems should not persist indefinitely simply because they
exist.

By planning for responsible retirement, organisations maintain control
over their technological infrastructure.

They ensure that outdated or inappropriate systems can be replaced
without undermining accountability or governance.

# Completing the Capability-Driven Development Lifecycle

The concept of system retirement completes the lifecycle of
Capability-Driven Development.

The method begins with defining **capability intent** and continues
through boundary design, ethical analysis, governance integration,
architectural design, evaluation, and responsible iteration.

Designing for system endings ensures that this lifecycle remains
complete.

Systems can emerge, evolve, and eventually be retired in ways that
preserve institutional capability and responsibility.

This perspective recognises that technological systems are not permanent
solutions. They are tools that support human and institutional
capability for a period of time.

Eventually, those tools must be replaced or reimagined.

By designing systems that can end responsibly, organisations ensure that
technological change remains aligned with the values and
responsibilities that guide their work.

Capability-Driven Development therefore concludes not with system
deployment, but with the recognition that responsible design includes
planning for how systems will eventually give way to the next generation
of responsible technologies.

# PART III

# Applying Capability-Driven Development

# Chapter 12

# Building Responsible Decision Support Systems

Decision support systems are among the most common and influential
applications of artificial intelligence within organisations.

Across domains such as healthcare, education, public services, research,
finance, and governance, decision support systems are used to analyse
complex information, highlight relevant patterns, and recommend possible
courses of action. These systems promise to enhance human judgement by
processing data at scales and speeds that would otherwise be impossible.

In principle, decision support systems are designed to **assist rather
than replace human decision-makers**.

In practice, however, many such systems gradually evolve into something
quite different.

Instead of supporting human judgement, they begin to shape it.
Recommendations become default decisions. Analytical outputs are
interpreted as objective truth. Professionals feel pressure to align
with algorithmic outputs even when their experience suggests alternative
interpretations.

Over time, decision support systems can quietly transform decision
processes in ways that undermine accountability and professional
capability.

Capability-Driven Development provides a framework for preventing these
outcomes.

By beginning with capability intent, defining human--AI boundaries,
embedding governance mechanisms, and designing architecture that
preserves human authority, CDD helps organisations build decision
support systems that genuinely enhance rather than erode institutional
capability.

This chapter illustrates how Capability-Driven Development can be
applied to the design of responsible decision support systems.

It focuses particularly on three risks that frequently emerge in such
systems:

- automation bias

- pseudo-objectivity

- accountability loss

# The Promise and Risk of Decision Support Systems

Decision support systems exist because many professional decisions
involve complex and uncertain information.

In healthcare, clinicians must interpret patient histories, diagnostic
tests, and treatment guidelines. In education, institutions analyse
student data to identify learning risks or opportunities. In research
management, teams assess funding proposals based on multiple criteria.

Artificial intelligence systems can assist in these contexts by:

- summarising large volumes of information

- identifying patterns within complex datasets

- generating alternative scenarios or predictions

- highlighting relevant evidence or precedents

These capabilities can significantly improve decision processes.

However, the same capabilities can also introduce new risks.

If decision support systems are designed poorly, they can alter how
professionals interpret information and exercise judgement.

Instead of supporting decision-makers, they may begin to influence or
even determine outcomes.

Understanding these risks is the first step toward designing responsible
systems.

# Automation Bias

One of the most well-documented risks in decision support systems is
**automation bias**.

Automation bias occurs when individuals place excessive trust in
automated outputs.

Even when professionals understand that algorithms are imperfect, the
presence of computational outputs can create a perception of authority
or objectivity. Numbers, rankings, and probability scores often appear
more definitive than human interpretation.

This perception can subtly influence behaviour.

Professionals may:

- accept system recommendations without fully examining underlying
  evidence

- overlook contradictory information

- assume that algorithmic outputs are based on more comprehensive
  analysis than their own judgement

Automation bias does not necessarily arise because users believe the
system is infallible.

Rather, it emerges because the system changes the **cognitive
environment** of decision-making.

When recommendations are presented prominently, they become anchors
around which judgement is formed.

Capability-Driven Development addresses automation bias by ensuring that
system design actively supports human interpretation rather than passive
acceptance of automated outputs.

# Pseudo-Objectivity

A second risk associated with decision support systems is
**pseudo-objectivity**.

Pseudo-objectivity occurs when algorithmic outputs appear objective even
though they are shaped by human assumptions, historical data, and
modelling choices.

Machine learning models often produce outputs that look precise---such
as probability scores or ranked recommendations. These outputs can
create the impression that the system is producing neutral, data-driven
conclusions.

In reality, these outputs reflect a series of design decisions.

Choices about which data to include, how variables are defined, and how
models are trained all influence system behaviour.

If these assumptions remain invisible to users, algorithmic outputs may
be interpreted as neutral facts rather than as analytical
interpretations.

Pseudo-objectivity can therefore distort decision-making by masking the
uncertainties and assumptions underlying system outputs.

Capability-Driven Development encourages system designs that make these
limitations visible.

# Accountability Loss

A third risk arises when decision support systems weaken
**accountability**.

In traditional decision processes, responsibility for outcomes is
typically associated with identifiable individuals or institutional
roles.

When AI systems influence decisions, responsibility may become more
diffuse.

Professionals may rely on system recommendations. Designers may argue
that users retain final authority. Organisations may claim that the
system merely provides analytical support.

In practice, responsibility may become unclear.

If a decision produces harmful consequences, organisations may struggle
to explain how the outcome occurred or who should be held accountable.

Capability-Driven Development addresses this problem by ensuring that
decision support systems preserve clear responsibility structures.

# Applying Capability-Driven Development

To illustrate how Capability-Driven Development addresses these risks,
consider a hypothetical decision support system designed to assist
professionals in evaluating complex cases.

Such a system might analyse relevant data, highlight important factors,
and generate recommendations for possible actions.

Applying CDD to this system involves several steps.

# Step 1: Defining Capability Intent

The design process begins by clarifying **capability intent**.

Rather than asking how the system can automate decision-making,
designers ask what capabilities the system should support.

For example, the system may aim to:

- help professionals review complex information efficiently

- highlight relevant patterns within large datasets

- support reflective and evidence-informed decision-making

These capabilities emphasise assistance rather than automation.

The system is intended to enhance human interpretation, not replace it.

Defining capability intent provides a reference point against which
future design decisions can be evaluated.

# Step 2: Defining Human--AI Boundaries

The next step is defining **human--AI boundaries**.

These boundaries clarify the roles of AI and human actors within the
decision process.

For a decision support system, the boundaries may specify that:

- the AI system analyses data and generates insights

- human professionals interpret those insights

- final decisions remain under human authority

The system may also include escalation mechanisms for complex cases and
override capabilities that allow professionals to challenge system
outputs.

These boundaries ensure that automated analysis does not become
automated decision-making.

# Step 3: Ethical and Risk Analysis

Designers must also examine ethical and operational risks.

Potential concerns might include:

- biases embedded in historical training data

- over-reliance on algorithmic outputs

- unequal impacts on different groups

A Risk and Misuse Register can document these issues and identify
mitigation strategies.

For example, system outputs may be accompanied by explanations or
contextual information that encourages critical interpretation.

# Step 4: Governance Integration

Governance mechanisms must also be integrated into system architecture.

This may include:

- recording when recommendations influence decisions

- logging override actions

- enabling governance bodies to review decision patterns

Such mechanisms ensure that system behaviour remains transparent and
accountable.

# Step 5: Architectural Design

The architecture of the system should reinforce the intended boundaries
between human and AI roles.

For example, recommendations may be presented as **analytical insights
rather than definitive answers**.

Interfaces may encourage users to review evidence before reaching
conclusions.

Automated outputs may appear alongside alternative interpretations or
contextual information.

These design choices reduce the risk of automation bias and
pseudo-objectivity.

# Example Workflow

Consider how a responsible decision support system might function in
practice.

1.  A professional submits a case for analysis.

2.  The system reviews relevant data and identifies key factors.

3.  Analytical outputs are presented in an interface designed to support
    interpretation.

4.  The professional reviews the information, considering both system
    insights and contextual knowledge.

5.  The professional reaches a decision and records the rationale.

In this workflow, the system enhances human capability without replacing
judgement.

# Monitoring System Behaviour

Even well-designed systems must be monitored over time.

Behavioural indicators---such as the frequency of overrides or patterns
of reliance on system recommendations---can reveal whether the system is
influencing decision processes in unintended ways.

If users begin treating automated outputs as authoritative, system
design may need to be adjusted.

Evaluation therefore plays an important role in maintaining responsible
decision support.

# Strengthening Institutional Capability

When decision support systems are designed through Capability-Driven
Development, they strengthen institutional capability rather than
weakening it.

Professionals gain access to improved analytical tools while retaining
authority over decisions.

Organisations maintain visibility into how decisions occur.

Governance bodies retain the ability to review and challenge system
behaviour.

Rather than replacing human judgement, AI becomes a partner in complex
decision processes.

# Decision Support as Responsible Human--AI Collaboration

Decision support systems represent one of the most promising
applications of artificial intelligence.

When designed responsibly, they can enhance human understanding, support
reflective judgement, and improve institutional decision-making.

However, achieving these outcomes requires more than technical
sophistication.

It requires system design that preserves capability, maintains
accountability, and supports governance.

Capability-Driven Development provides the structure needed to achieve
these goals.

By beginning with capability intent and maintaining responsibility
throughout the system lifecycle, organisations can build decision
support systems that genuinely serve the humans and institutions that
rely upon them.

Such systems do not automate judgement.

They support it.

# Chapter 13

# Designing Workflow Orchestration Systems

Many of the most influential AI systems in modern organisations are not
decision systems.

They are coordination systems.

These systems do not determine final outcomes directly. Instead, they
organise work. They route tasks, prioritise cases, connect data sources,
and trigger actions across multiple actors and services. In doing so,
they shape how decisions are reached.

Workflow orchestration systems increasingly operate at the centre of
organisational infrastructure.

Examples include:

- case management systems in healthcare and public services

- research administration and grant management workflows

- compliance monitoring systems

- institutional service desks and support platforms

- automated operational pipelines in large organisations

In recent years, these systems have begun to incorporate artificial
intelligence in several ways. AI models may classify incoming requests,
prioritise tasks, generate summaries, detect anomalies, or suggest next
steps within workflows.

More recently, **agentic AI systems** have begun to extend these
capabilities further. Instead of producing isolated outputs, AI agents
may coordinate actions across multiple tools, services, and data
sources.

These developments significantly expand the influence of workflow
orchestration systems.

While decision support systems influence how individuals interpret
information, orchestration systems influence **how work itself
unfolds**.

For this reason, workflow orchestration systems represent a particularly
important domain for Capability-Driven Development.

Poorly designed orchestration systems can obscure responsibility, create
brittle processes, and introduce hidden automation into critical
workflows. Well-designed systems can strengthen coordination, clarify
accountability, and support responsible collaboration between humans and
AI systems.

This chapter explores how Capability-Driven Development can guide the
design of responsible workflow orchestration systems.

It focuses on three key aspects:

- coordination systems

- escalation design

- responsibility in distributed workflows

The chapter also examines how these principles apply to emerging
**agentic AI orchestration systems**.

# Understanding Coordination Systems

Workflow orchestration systems exist to coordinate complex processes.

In many organisations, work involves multiple actors performing
interdependent tasks. Information flows between teams, systems, and
decision-makers. Tasks must be prioritised, assigned, and monitored.

Without coordination mechanisms, these processes become fragmented and
inefficient.

Coordination systems provide structure.

They typically perform functions such as:

- routing tasks to appropriate actors

- prioritising work according to defined criteria

- tracking workflow progress

- triggering subsequent actions when tasks are completed

- integrating information across systems

In traditional systems, these functions were often rule-based.

For example, a workflow might assign cases according to predefined
criteria such as location, department, or priority level.

AI-enabled orchestration systems extend these capabilities by
incorporating data-driven analysis.

AI components may:

- classify incoming requests

- predict urgency or risk levels

- identify anomalies within workflow patterns

- generate summaries to assist human reviewers

These capabilities can improve coordination efficiency. However, they
also introduce new risks if the orchestration system begins shaping
decision processes in unintended ways.

# When Coordination Becomes Decision

A key challenge in workflow orchestration systems is the **boundary
between coordination and decision-making**.

Coordination systems are typically intended to organise work rather than
determine outcomes. However, the structure of coordination can
significantly influence decisions.

For example, consider a workflow system that prioritises cases according
to an algorithmic risk score.

Although the system does not formally decide outcomes, the
prioritisation determines which cases receive attention first. In
practice, this can strongly influence final decisions.

Similarly, an orchestration system that automatically routes requests to
specific teams may shape how those requests are interpreted or resolved.

These dynamics illustrate an important insight:

Coordination systems often exercise indirect decision power.

For this reason, workflow orchestration systems must be designed with
the same care and governance considerations as decision support systems.

Capability-Driven Development helps ensure that coordination structures
remain aligned with institutional responsibility.

# Human--AI Boundaries in Orchestration Systems

The first step in designing a responsible orchestration system is
defining **human--AI boundaries** within workflows.

These boundaries clarify which parts of the workflow can be automated
and which require human judgement.

For example, AI systems may assist with:

- classifying incoming tasks

- summarising information for review

- detecting patterns or anomalies within workflows

However, tasks involving interpretation, ethical judgement, or
institutional responsibility should remain under human authority.

Defining these boundaries ensures that coordination does not silently
become automated decision-making.

# Escalation Design

One of the most important aspects of workflow orchestration systems is
**escalation design**.

Escalation mechanisms determine how workflows respond to uncertainty,
complexity, or potential harm.

In many systems, escalation processes are poorly defined. Cases may
remain within automated workflows even when human intervention is
necessary.

Capability-Driven Development treats escalation as a core design
feature.

Escalation mechanisms should address questions such as:

- When should automated processes pause for human review?

- What signals indicate that escalation is required?

- Who receives escalated cases?

- How are escalated cases documented and resolved?

Examples of escalation triggers may include:

- conflicting data signals

- unusually high-risk classifications

- ambiguous or incomplete inputs

- ethical concerns raised by users

Effective escalation design ensures that human judgement can intervene
when automated coordination becomes insufficient.

# Responsibility in Distributed Workflows

Workflow orchestration systems often involve **distributed
responsibility**.

Multiple actors may interact with the system at different stages of the
workflow. Tasks may move across departments, teams, or organisational
units.

In such environments, responsibility can become difficult to trace.

For example, if a workflow produces an undesirable outcome, several
actors may have influenced the process:

- the system that routed the task

- the professional who reviewed the information

- the team responsible for resolving the case

Without clear documentation, it may be difficult to determine where
responsibility lies.

Capability-Driven Development addresses this challenge by ensuring that
workflow systems support **responsibility traceability**.

This involves recording key events within the workflow, including:

- task routing decisions

- human interactions with system outputs

- escalation events

- overrides or adjustments to workflow logic

Such records allow organisations to reconstruct how workflows unfolded.

# Architectural Patterns for Responsible Orchestration

Several architectural patterns can help preserve responsibility and
oversight in orchestration systems.

### Assisted Routing

In assisted routing architectures, AI systems recommend task assignments
but allow human operators to confirm or adjust those assignments.

### Conditional Automation

Certain tasks may be automated under normal conditions but require human
confirmation when risk indicators are present.

### Escalation Pathways

Clear pathways allow cases to move from automated workflows to human
review when necessary.

### Transparent Logging

Workflow events are recorded to support monitoring, evaluation, and
governance review.

These patterns ensure that coordination remains transparent and
governable.

# Agentic AI and Workflow Orchestration

Recent developments in AI have introduced a new class of systems often
described as **agentic AI systems**.

Agentic systems differ from traditional AI tools in that they can
perform sequences of actions across multiple systems. They may retrieve
information, generate outputs, trigger workflows, and interact with
external tools autonomously.

In many cases, agentic AI systems function as orchestration layers.

For example, an AI agent may:

- retrieve relevant information from multiple databases

- generate summaries for human review

- trigger follow-up actions in workflow systems

- coordinate interactions between services

These capabilities offer powerful new possibilities for organisational
coordination.

However, they also increase the importance of responsible system design.

When AI agents coordinate actions across multiple systems, their
influence on workflows becomes substantial. Poorly designed agentic
systems may obscure responsibility or create unpredictable behaviour.

Capability-Driven Development provides an important framework for
addressing these challenges.

# Designing Responsible Agentic Orchestration

Applying Capability-Driven Development to agentic orchestration systems
involves several considerations.

### Capability Intent

The system's purpose should be clearly defined. Agentic systems should
enhance coordination rather than replace institutional judgement.

### Human--AI Boundaries

Agents may automate routine coordination tasks but should not exercise
authority over decisions requiring human responsibility.

### Escalation Mechanisms

Agentic systems must include clear pathways for human intervention when
unexpected situations arise.

### Governance Visibility

Actions performed by agents should be logged and reviewable.

These principles ensure that agentic orchestration systems remain
accountable and transparent.

# Monitoring Orchestration Systems

Once deployed, orchestration systems should be evaluated continuously.

Monitoring indicators may include:

- patterns of workflow routing

- frequency of escalations

- response times for critical cases

- instances of workflow overrides

These indicators help reveal whether the system supports coordination
effectively or introduces new risks.

# Strengthening Organisational Coordination

When designed responsibly, workflow orchestration systems can
significantly strengthen organisational capability.

They can improve information flow, reduce delays, and support
collaboration across complex environments.

However, these benefits depend on systems that preserve responsibility,
support escalation, and maintain transparency.

Capability-Driven Development provides the design principles needed to
achieve this balance.

# Orchestration as Institutional Infrastructure

Workflow orchestration systems increasingly form the backbone of
organisational infrastructure.

They coordinate tasks across departments, integrate data flows, and
support complex decision processes.

Because of this central role, their design has profound implications for
governance and institutional responsibility.

By applying Capability-Driven Development to orchestration
systems---particularly those incorporating agentic AI---organisations
can ensure that coordination technologies remain aligned with human
judgement and institutional accountability.

In doing so, they create systems that enhance organisational capability
rather than quietly reshaping it in ways that undermine responsibility.

The final chapter examines how these principles extend to broader
monitoring and oversight systems that support governance across entire
organisational infrastructures.

# Chapter 14

# Monitoring Without Surveillance

Modern organisations increasingly rely on monitoring systems.

These systems track performance, detect anomalies, identify risks, and
provide oversight across complex institutional processes. In sectors
such as healthcare, research, education, public administration, and
finance, monitoring systems have become essential tools for maintaining
operational integrity and governance accountability.

Artificial intelligence is rapidly expanding the capabilities of such
systems.

AI-enabled monitoring tools can analyse large volumes of activity data,
identify unusual patterns, detect potential risks earlier than manual
processes, and generate insights that help institutions maintain
oversight over complex operations.

When used responsibly, monitoring systems can strengthen institutional
capability. They allow organisations to detect emerging issues, respond
to risks, and improve decision processes.

However, monitoring systems also introduce an important tension.

Monitoring intended to support governance can easily drift into
**surveillance**.

Systems designed to observe processes may begin observing individuals.
Tools created to identify operational risks may be used to evaluate
personal behaviour or performance. Data collected for institutional
oversight may gradually be repurposed for disciplinary or managerial
control.

This phenomenon---often referred to as **surveillance creep**---poses
serious ethical and governance challenges.

Capability-Driven Development provides a framework for designing
monitoring systems that strengthen governance while avoiding
surveillance dynamics.

This chapter explores how monitoring and oversight systems can be
designed responsibly by focusing on three key elements:

- governance dashboards

- anomaly detection systems

- ethical monitoring practices

It also examines how surveillance creep occurs and how responsible
system design can prevent it.

# The Purpose of Monitoring Systems

Monitoring systems exist to provide **institutional visibility**.

In complex organisations, many processes occur simultaneously across
different teams, departments, and technologies. Without structured
monitoring, it becomes difficult to understand how these processes
interact or where potential problems may emerge.

Monitoring systems provide several important capabilities.

They may:

- track workflow activity across systems

- identify unusual patterns in operational data

- monitor system performance and reliability

- surface indicators of risk or failure

- support governance review and oversight

These capabilities help organisations maintain awareness of their
operational environment.

However, monitoring systems must be designed carefully.

If they are poorly designed, they can create cultures of surveillance
rather than systems of responsible oversight.

# Governance Monitoring vs Surveillance

The difference between governance monitoring and surveillance lies in
**purpose and design**.

Governance monitoring focuses on institutional processes.

Its goal is to ensure that systems operate responsibly, risks are
identified early, and organisations retain the ability to intervene when
necessary.

Surveillance systems, by contrast, focus on individuals.

They monitor behaviour in ways that may be intrusive, punitive, or
disproportionate to the legitimate needs of governance.

For example, a monitoring system designed to detect workflow bottlenecks
may analyse aggregate task completion patterns across departments. Such
analysis helps organisations understand where coordination challenges
arise.

However, if the same system begins ranking individual staff members
according to productivity metrics derived from those workflows, it may
shift from governance monitoring to surveillance.

Capability-Driven Development encourages designers to define monitoring
systems in ways that support **institutional oversight rather than
individual surveillance**.

# Governance Dashboards

One of the most common forms of monitoring infrastructure is the
**governance dashboard**.

Governance dashboards provide visual summaries of system activity,
allowing organisations to observe patterns across workflows and
processes.

In responsible systems, governance dashboards are designed to support
oversight without overwhelming users with raw data.

Effective dashboards typically present indicators such as:

- workflow volumes and trends

- escalation rates

- override frequencies

- system performance metrics

- anomaly alerts

These indicators allow governance bodies to understand how systems
behave over time.

For example, an unusually high rate of escalation events may signal that
automated processes are encountering cases beyond their intended scope.
Similarly, declining override rates may indicate growing reliance on
automated recommendations.

By presenting such indicators clearly, governance dashboards enable
organisations to monitor system behaviour without requiring detailed
technical analysis.

# Designing Responsible Governance Dashboards

Governance dashboards should be designed with several principles in
mind.

### Aggregation

Indicators should emphasise aggregated patterns rather than individual
behaviour unless individual accountability is explicitly required.

### Interpretability

Metrics should be presented in ways that support meaningful
interpretation rather than superficial comparisons.

### Context

Indicators should be accompanied by contextual information that helps
users understand what the data represents.

### Governance Relevance

Dashboards should prioritise metrics that relate directly to
institutional oversight and responsibility.

By following these principles, governance dashboards support oversight
without encouraging surveillance.

# Anomaly Detection

Another important function of monitoring systems is **anomaly
detection**.

Anomaly detection systems identify unusual patterns within operational
data.

AI techniques are particularly well suited for this purpose because they
can analyse large datasets and identify deviations that might not be
immediately visible to human observers.

Examples of anomalies may include:

- unexpected spikes in workflow activity

- unusual patterns of automated classifications

- deviations in system performance

- inconsistencies in data flows across systems

Detecting such anomalies allows organisations to investigate potential
issues before they escalate into larger problems.

However, anomaly detection systems must be designed carefully to ensure
that alerts support governance rather than generate noise or unjustified
suspicion.

# Interpreting Anomalies

An anomaly does not necessarily indicate wrongdoing or failure.

In many cases, unusual patterns reflect legitimate changes in
organisational activity.

For example, a surge in case submissions may occur because of seasonal
demand. A sudden increase in escalations may reflect heightened caution
by users responding to new policy guidance.

Monitoring systems should therefore treat anomalies as **signals for
investigation rather than conclusions**.

Alerts should prompt human review rather than trigger automatic
responses.

Capability-Driven Development encourages anomaly detection systems that
support interpretive judgement rather than automated enforcement.

# Ethical Monitoring Systems

Responsible monitoring systems must also address ethical considerations.

Monitoring technologies can easily become intrusive if their scope is
not carefully defined.

Capability-Driven Development therefore emphasises the concept of
**ethical monitoring systems**.

Ethical monitoring systems are designed with several safeguards.

### Purpose Limitation

Data collection should be limited to information necessary for
governance and oversight.

### Transparency

Stakeholders should understand what is being monitored and why.

### Proportionality

Monitoring practices should be proportionate to the risks being managed.

### Governance Oversight

Monitoring systems themselves should be subject to review by governance
bodies.

These safeguards ensure that monitoring supports institutional
responsibility without undermining trust.

# Surveillance Creep

One of the greatest risks associated with monitoring systems is
**surveillance creep**.

Surveillance creep occurs when monitoring systems gradually expand
beyond their original purpose.

This expansion may occur through several mechanisms.

### Scope Expansion

Data collected for operational oversight may begin to be used for
evaluating individual performance.

### Feature Accumulation

Additional monitoring capabilities may be added incrementally without
reconsidering ethical implications.

### Data Repurposing

Information collected for governance may be reused for unrelated
purposes.

### Cultural Shift

Organisational cultures may begin to treat monitoring tools as
instruments of control rather than oversight.

These dynamics can transform governance systems into surveillance
infrastructures.

Preventing surveillance creep requires explicit design constraints and
governance review.

# Designing Systems That Resist Surveillance Creep

Capability-Driven Development provides several mechanisms that help
prevent surveillance creep.

### Explicit Scope Definition

Monitoring systems should clearly define what is being monitored and
why.

### Governance Boundaries

Policies should restrict how monitoring data can be used.

### Oversight Review

Governance bodies should periodically review monitoring systems to
ensure they remain aligned with their intended purpose.

### Architectural Safeguards

System architecture may limit access to sensitive monitoring data or
prevent certain forms of analysis.

These mechanisms ensure that monitoring remains aligned with governance
needs.

# Monitoring as Institutional Learning

Monitoring systems also play an important role in organisational
learning.

By observing patterns across workflows and decision processes,
organisations can identify opportunities for improvement.

For example, monitoring may reveal:

- recurring workflow bottlenecks

- areas where escalation mechanisms are frequently used

- patterns of system misuse or misunderstanding

These insights can inform system redesign, training programmes, or
governance reforms.

Monitoring therefore supports continuous improvement rather than simply
detecting problems.

# Monitoring and Trust

Perhaps the most important consideration in monitoring system design is
**trust**.

Monitoring systems that appear intrusive or punitive may undermine trust
among those who interact with them.

Conversely, monitoring systems designed transparently and responsibly
can strengthen institutional trust.

When stakeholders understand that monitoring exists to support
governance and protect organisational integrity, they are more likely to
engage constructively with such systems.

Capability-Driven Development emphasises monitoring designs that respect
this balance.

# Monitoring as Responsible Oversight

Monitoring systems are essential components of responsible AI-enabled
organisations.

They provide visibility into complex processes, support governance
oversight, and help organisations detect emerging risks.

However, their design must ensure that monitoring strengthens
institutional capability rather than creating surveillance dynamics.

By focusing on governance dashboards, responsible anomaly detection, and
ethical monitoring practices, organisations can create systems that
support oversight without undermining trust.

Such systems reinforce the central goal of Capability-Driven
Development:

to build technological infrastructures that enhance human and
institutional responsibility rather than eroding it.

With this final example, the practical applications of Capability-Driven
Development across decision systems, workflow orchestration systems, and
monitoring infrastructures become clear.

Together, these examples illustrate how capability-centred design can
guide the development of AI-enabled systems that remain accountable,
governable, and aligned with human judgement.

# PART IV

# Capability-Driven Development in Practice

# Chapter 15

# Implementing Capability-Driven Development in Organisations

Capability-Driven Development (CDD) is not intended to replace existing
engineering practices.

Most organisations already use structured development methods such as
Agile, DevOps, product lifecycle management, or enterprise architecture
frameworks. These approaches provide valuable tools for planning,
building, and maintaining technical systems.

However, many of these methods were created before artificial
intelligence systems began influencing decision processes at scale.

As a result, they often focus primarily on technical performance,
feature delivery, and operational efficiency. Questions of capability
preservation, governance integration, and responsibility design may
appear only indirectly.

CDD complements these existing methods by introducing a
**capability-centred perspective**.

Rather than replacing development practices, CDD adds a structured layer
that ensures systems are designed, evaluated, and evolved in ways that
preserve human judgement and institutional responsibility.

Implementing CDD within organisations therefore requires attention to
several practical dimensions:

- the composition of design teams

- the role of governance bodies

- the structure of review processes

- integration with existing development workflows

This chapter provides guidance on how organisations can introduce
Capability-Driven Development into real operational environments.

# From Method to Practice

Many conceptual frameworks fail because they remain disconnected from
day-to-day organisational practices.

CDD is designed to avoid this problem.

Its principles are expressed through practical artefacts and processes
introduced throughout the system lifecycle.

These artefacts include:

- the System Capability Brief

- the Human--AI Boundary Map

- the Risk and Misuse Register

- the Governance and Oversight Plan

Together, these documents provide a structured way to connect system
design decisions with capability and governance considerations.

However, creating these artefacts requires collaboration across multiple
organisational roles.

Successful implementation therefore depends on **how teams work
together**.

# Designing Effective System Design Teams

AI-enabled systems rarely exist within purely technical domains.

They influence professional judgement, organisational workflows, and
governance responsibilities.

For this reason, CDD encourages **multidisciplinary design teams**.

Such teams typically include several types of expertise.

### Technical Engineers

Engineers design and implement system architecture, models, and
infrastructure.

### Domain Experts

Professionals who understand the institutional context in which the
system will operate.

### Governance and Compliance Specialists

Individuals responsible for regulatory alignment, risk management, and
ethical oversight.

### Product or Service Designers

Experts who shape system interfaces and user interactions.

Bringing these perspectives together ensures that system design
decisions consider both technical feasibility and institutional
responsibility.

# The Role of Domain Expertise

Domain expertise plays a particularly important role in CDD.

AI systems often operate within professional environments where
decisions require contextual understanding.

For example:

- clinicians interpret medical evidence

- educators evaluate learning progress

- researchers assess methodological rigour

If system design occurs without domain expertise, automated outputs may
be interpreted incorrectly or applied in ways that undermine
professional judgement.

Domain experts therefore contribute to:

- defining capability intent

- identifying ethical risks

- clarifying decision boundaries

Their involvement helps ensure that systems support rather than displace
professional expertise.

# Governance Bodies as Design Partners

In many organisations, governance bodies operate separately from system
design processes.

Oversight committees may review systems only after development has been
completed.

This separation can create challenges.

If governance concerns emerge late in development, addressing them may
require significant redesign.

Capability-Driven Development therefore encourages governance bodies to
become **design partners rather than external reviewers**.

Early engagement allows governance stakeholders to shape system
architecture before critical design decisions are finalised.

Governance bodies may contribute to:

- reviewing capability intent

- evaluating risk and misuse scenarios

- defining oversight mechanisms

- approving scope boundaries

This collaboration ensures that governance considerations are integrated
into system design rather than added as an afterthought.

# Structuring Review Processes

Implementing CDD also requires structured review processes throughout
the development lifecycle.

These reviews help ensure that system evolution remains aligned with
capability and governance principles.

Several review stages are particularly important.

### Capability Intent Review

At the beginning of a project, stakeholders review the System Capability
Brief to ensure that system purpose and capability goals are clearly
defined.

### Boundary Review

Human--AI boundaries are examined to confirm that decision authority
remains appropriately distributed.

### Risk and Ethics Review

Potential harms and misuse scenarios documented in the Risk and Misuse
Register are evaluated.

### Governance Review

The Governance and Oversight Plan is assessed to ensure that
accountability and auditability mechanisms are adequate.

These reviews provide checkpoints where design decisions can be
reconsidered before systems become operational.

# Integrating CDD with Agile Development

Many organisations rely on Agile development practices.

Agile emphasises rapid iteration, continuous improvement, and close
collaboration between developers and stakeholders.

CDD can integrate effectively with Agile workflows.

For example:

- the System Capability Brief may guide the creation of initial product
  backlogs

- human--AI boundaries can inform user stories and acceptance criteria

- risk registers may be revisited during sprint reviews

- governance indicators can be incorporated into monitoring dashboards

Rather than slowing development, these artefacts help teams maintain
clarity about system responsibilities during rapid iteration cycles.

# Integrating CDD with DevOps Practices

DevOps practices focus on continuous integration, deployment, and
operational monitoring.

CDD complements DevOps by ensuring that governance considerations extend
into operational environments.

For example:

- logging systems introduced for auditability support monitoring
  pipelines

- evaluation indicators may be integrated into operational dashboards

- governance alerts can be incorporated into system monitoring tools

This integration allows organisations to maintain oversight as systems
evolve through continuous deployment processes.

# Documentation and Institutional Memory

One of the most valuable aspects of CDD is its emphasis on
**documentation that supports institutional memory**.

Many organisations struggle to maintain clear records of how complex
systems were designed or how responsibilities were distributed.

Over time, staff turnover and system modifications can make it difficult
to understand how systems operate.

CDD artefacts provide structured documentation that records key design
decisions.

These records support:

- governance review

- system evaluation

- future system redesign

They also help organisations demonstrate accountability to regulators,
auditors, or external stakeholders.

# Training and Capability Development

Implementing CDD requires that organisations develop the necessary
capabilities among their staff.

Designers and engineers must learn how to consider governance and
capability implications during system development. Governance
professionals must become familiar with technical architectures that
shape system behaviour.

Training programmes can help build these shared capabilities.

Such programmes may include:

- workshops on human--AI boundary design

- training on risk identification and misuse analysis

- guidance on interpreting governance dashboards

- cross-disciplinary discussions between technical and governance teams

Developing these capabilities strengthens the organisation's ability to
design responsible systems.

# Embedding CDD in Organisational Culture

For CDD to succeed, it must become part of organisational culture.

This means recognising that system design is not purely a technical
activity.

Instead, it is a collaborative process that shapes how institutions
exercise responsibility.

Organisations that embrace this perspective often demonstrate several
characteristics.

They encourage open discussion about system risks and limitations. They
value transparency in decision processes. They treat governance not as
an obstacle but as a design partner.

Such cultures support the long-term sustainability of responsible AI
systems.

# Implementing CDD Incrementally

Organisations do not need to adopt Capability-Driven Development all at
once.

Many begin by introducing selected elements into existing projects.

For example, teams might initially adopt the System Capability Brief to
clarify project goals. Later, they may introduce Human--AI Boundary Maps
for systems that influence decision processes.

Over time, additional artefacts and review processes can be integrated
as organisational capability grows.

This incremental approach allows organisations to experiment with CDD
while adapting it to their specific contexts.

# CDD as Institutional Capability

Ultimately, Capability-Driven Development should be understood not only
as a design method but also as an **institutional capability**.

Organisations that adopt CDD develop the ability to:

- design AI systems responsibly

- maintain governance visibility over complex infrastructures

- adapt systems as technologies evolve

- preserve human and institutional capability over time

These abilities are increasingly important as artificial intelligence
becomes embedded within organisational decision processes.

CDD provides the structure needed to support these capabilities.

# Toward Responsible Human--AI Systems

The implementation of Capability-Driven Development marks a shift in how
organisations approach technological innovation.

Rather than focusing solely on what AI systems can do, CDD encourages
organisations to ask a more fundamental question:

What capabilities must remain intact when AI becomes part of
institutional infrastructure?

By organising system design around this question, organisations can
ensure that AI technologies enhance rather than undermine their ability
to act responsibly.

Capability-Driven Development therefore represents not only a method for
building better systems but also a framework for sustaining responsible
institutions in an increasingly AI-enabled world.

# Chapter 16

# The Future of Governable AI Systems

Artificial intelligence is rapidly becoming part of the infrastructure
of modern institutions.

In earlier phases of technological development, AI systems were often
treated as experimental tools. Organisations explored machine learning
models to analyse datasets, automate narrow tasks, or generate
predictive insights. These systems were often peripheral to core
institutional operations.

That situation is changing.

AI systems are increasingly embedded in the everyday processes that
shape decisions, allocate resources, coordinate work, and monitor
organisational activity. From public services and healthcare to research
management and education, intelligent systems are beginning to influence
how institutions function.

This shift brings both opportunity and responsibility.

Artificial intelligence can enhance human capability, support more
informed decision-making, and improve organisational coordination. At
the same time, it introduces new risks: automation bias, opaque decision
processes, governance gaps, and the erosion of professional judgement.

As these systems become more powerful and more integrated into
institutional infrastructure, organisations face an urgent question:

How can AI systems remain governable?

Capability-Driven Development is one response to this challenge. It
represents part of a broader movement toward designing AI systems that
strengthen human capability rather than displacing it.

This chapter explores how CDD connects with three emerging ideas that
are shaping the future of responsible AI systems:

- human--AI capability

- governance-aware engineering

- responsible system design

Together, these ideas point toward a new approach to technological
development---one in which systems are designed not only for performance
but also for accountability, transparency, and institutional
responsibility.

# From Tools to Infrastructure

One of the most significant developments in the evolution of AI is the
transition from **tools to infrastructure**.

In earlier phases, AI systems were used as specialised analytical tools.
They supported particular tasks, such as image recognition, language
processing, or predictive modelling.

Today, AI systems are increasingly integrated into broader operational
systems.

They coordinate workflows, monitor institutional processes, and assist
decision-making across complex environments.

When AI systems operate at this level, their influence extends beyond
individual tasks.

They shape how organisations:

- interpret information

- coordinate work

- allocate attention and resources

- exercise authority

In effect, AI becomes part of the **governance infrastructure** of
institutions.

This transformation requires new approaches to system design.

Traditional engineering practices emphasise efficiency, reliability, and
scalability. These goals remain important, but they are no longer
sufficient.

When AI systems influence institutional processes, they must also
support governance.

# The Emergence of Human--AI Capability

One response to this challenge is the concept of **human--AI
capability**.

Human--AI capability refers to the ability of individuals, teams, and
institutions to work effectively and responsibly with artificial
intelligence.

This capability includes several dimensions.

It involves understanding how AI systems function, recognising their
limitations, and interpreting their outputs critically. It also involves
designing workflows in which AI supports human judgement rather than
replacing it.

At the institutional level, human--AI capability includes the ability to
govern AI systems responsibly, ensuring that decisions remain
accountable and transparent.

The **AI Capability Framework** was developed to support this broader
vision.

The framework identifies several domains that organisations must develop
in order to work effectively with AI. These include awareness of AI
systems, responsible collaboration between humans and AI, ethical
understanding, governance practices, and continuous learning.

However, frameworks that describe capability are only part of the
solution.

Organisations also need methods for designing systems that **preserve
and strengthen those capabilities**.

Capability-Driven Development addresses this need.

# Governance-Aware Engineering

Another emerging idea shaping the future of AI systems is
**governance-aware engineering**.

Governance-aware engineering recognises that technical systems
increasingly influence institutional authority and responsibility.

As a result, system design must consider governance implications from
the beginning.

This represents a shift from earlier approaches where governance was
treated as an external layer applied after systems were built.

In governance-aware engineering, governance mechanisms are embedded
directly into system architecture.

Systems are designed to support:

- accountability

- auditability

- contestability

- oversight

Capability-Driven Development embodies this perspective.

By integrating governance considerations throughout the system
lifecycle---from capability intent to architecture design and
evaluation---CDD ensures that governance becomes part of the system
itself.

This approach is particularly important as AI systems become more
autonomous and interconnected.

# Responsible System Design

A third concept shaping the future of AI is **responsible system
design**.

Responsible system design recognises that technological systems
influence social and institutional outcomes. As a result, designers must
consider not only what systems can do but also how they shape human
behaviour and organisational practices.

Responsible system design involves several principles.

First, systems should preserve human agency and judgement.

Second, they should support transparency and explainability.

Third, they should enable governance and oversight.

Fourth, they should be adaptable and open to evaluation as technologies
evolve.

Capability-Driven Development translates these principles into practical
design steps.

By beginning with capability intent and maintaining responsibility
throughout the system lifecycle, CDD helps ensure that AI systems remain
aligned with institutional values.

# Connecting CDD to the AI Capability Framework

Capability-Driven Development is closely connected to the **AI
Capability Framework**.

The AI Capability Framework describes the capabilities that individuals
and institutions must develop to work responsibly with AI.

These capabilities include:

- awareness of AI systems and their limitations

- collaboration between humans and AI technologies

- ethical reasoning and impact awareness

- governance and decision accountability

- continuous reflection and learning

However, the framework intentionally remains **technology-neutral**.

It does not prescribe how systems should be built.

CDD complements the framework by providing a method for translating
capability principles into system design.

If the AI Capability Framework defines what responsible capability looks
like, Capability-Driven Development defines how systems can be designed
to preserve and strengthen that capability.

Together, these approaches form a coherent model for responsible AI
adoption.

# Connecting CDD to Human--AI Governance Engineering

Capability-Driven Development is also closely aligned with the emerging
discipline of **Human--AI Governance Engineering**.

Human--AI Governance Engineering focuses on how institutions can design
decision systems in which humans and AI collaborate responsibly.

It examines issues such as:

- decision authority

- accountability structures

- governance mechanisms

- institutional oversight of AI systems

Where Human--AI Governance Engineering focuses on governance structures
and institutional decision systems, CDD focuses on **how the systems
themselves are designed**.

The two approaches therefore operate at complementary levels.

Human--AI Governance Engineering addresses the broader governance
environment in which AI systems operate.

Capability-Driven Development provides the design method for building
systems that function responsibly within that environment.

Together, they form part of a broader intellectual movement toward
**governable AI systems**.

# Toward Governable AI Infrastructure

As AI technologies continue to evolve, the challenge facing
organisations will not simply be adopting new tools.

It will be designing infrastructures that remain **governable over
time**.

Governable systems must allow institutions to:

- understand how decisions occur

- challenge automated outputs

- adapt systems as contexts change

- maintain accountability for outcomes

Without these capabilities, organisations risk becoming dependent on
systems they cannot fully understand or control.

Capability-Driven Development helps address this risk by ensuring that
responsibility remains visible within system architecture.

# The Future of Capability-Centred Design

Looking forward, several trends are likely to shape the future of
capability-centred system design.

AI systems will become more autonomous and capable of coordinating
complex processes. Agentic AI systems will increasingly orchestrate
workflows across multiple tools and services. Monitoring systems will
analyse vast quantities of operational data in real time.

These developments will increase both the power and the complexity of
AI-enabled infrastructures.

In such environments, traditional governance approaches will struggle to
keep pace.

Design methods such as Capability-Driven Development will therefore
become increasingly important.

They provide a way to ensure that technological systems remain aligned
with human judgement and institutional responsibility even as AI
capabilities expand.

# A Different Vision of Technological Progress

The emergence of methods like CDD reflects a broader shift in how
technological progress is understood.

In earlier narratives, progress was often measured in terms of
automation: how many tasks machines could perform more efficiently than
humans.

Today, a different vision is beginning to emerge.

In this vision, technological progress is measured not by how much human
activity can be automated, but by how effectively technology can
**strengthen human capability and institutional responsibility**.

Artificial intelligence becomes not a replacement for human judgement
but a partner in complex decision processes.

Capability-Driven Development contributes to this vision by providing
practical tools for designing systems that support this partnership.

# Designing Systems Worth Trusting

Ultimately, the future of AI systems will depend on trust.

Institutions must trust that the systems they deploy will behave
responsibly. Professionals must trust that AI tools support rather than
undermine their expertise. Individuals affected by these systems must
trust that decisions remain accountable and transparent.

Trust cannot be created through policy statements alone.

It emerges from systems that are designed to make responsibility
visible, authority clear, and governance possible.

Capability-Driven Development represents one step toward building such
systems.

By placing human capability and institutional responsibility at the
centre of system design, it helps ensure that artificial intelligence
becomes not a source of institutional fragility but a foundation for
stronger, more accountable systems.

In that sense, the future of governable AI systems will not depend
solely on advances in technology.

It will depend on our ability to design systems that remain aligned with
the human and institutional capabilities they are meant to serve.

Appendix

# CDD Design Artifacts Toolkit

Capability-Driven Development (CDD) translates principles about
responsibility, capability, and governance into **practical design
artefacts**.

Throughout this book, several artefacts have been introduced that help
designers, engineers, and governance teams document how human--AI
systems are intended to operate. These artefacts provide structured ways
to record key design decisions and ensure that systems remain
understandable, accountable, and governable over time.

The CDD Design Artifacts Toolkit brings these elements together.

Each artefact serves a specific purpose within the lifecycle of a
system. Some are created at the beginning of a project to clarify intent
and responsibilities. Others support evaluation, monitoring, or
long-term institutional learning.

Importantly, these artefacts are not intended to create unnecessary
documentation. Instead, they provide **minimal but essential records**
that make system design visible to the people responsible for governing
and maintaining those systems.

Together, they form a lightweight governance infrastructure that can
accompany AI systems throughout their lifecycle.

The core artefacts in the CDD toolkit are:

- System Capability Brief

- Human--AI Boundary Map

- Risk and Misuse Register

- Governance and Oversight Plan

- Evaluation Log

- Retirement Notes

Each artefact addresses a specific challenge in designing responsible AI
systems.

# System Capability Brief

The **System Capability Brief** is the starting point for
Capability-Driven Development.

Before any system architecture is designed or automation is introduced,
organisations must clarify **what capability the system is intended to
support**.

Many AI projects begin with a focus on technological possibilities
rather than institutional needs. Teams may explore new models or
automation tools without fully considering how those technologies affect
professional judgement, governance responsibilities, or organisational
capability.

The System Capability Brief addresses this problem by requiring
designers to define the **capability intent** of the system.

This brief typically includes several key elements.

### Purpose of the System

The brief describes the organisational problem the system is intended to
address.

Rather than focusing on technology, the description emphasises the human
or institutional capability the system should support.

### Capability Goals

Designers identify the capabilities that the system should strengthen or
preserve.

These may include professional judgement, coordination between teams,
transparency in decision processes, or improved access to relevant
information.

### Risks of Capability Erosion

The brief also considers how the system could unintentionally weaken the
capabilities it is meant to support.

For example, a system that summarises complex information might reduce
professionals' opportunities to engage directly with underlying
evidence.

### Boundaries of Automation

Initial assumptions about where automation may or may not be appropriate
are also recorded.

These boundaries will later be refined through the Human--AI Boundary
Map.

The System Capability Brief ensures that system design begins with a
clear understanding of **what must be protected** as AI becomes part of
the workflow.

# Human--AI Boundary Map

The **Human--AI Boundary Map** defines how responsibilities are
distributed between human actors and AI systems.

Many AI systems fail to clarify these boundaries explicitly. As a
result, responsibility may gradually shift toward automated outputs even
when the system was originally intended to support human judgement.

The Human--AI Boundary Map prevents this problem by documenting the
**division of authority within the system**.

This map typically identifies several components.

### Decision Points

Key points within workflows where decisions occur are identified.

Each decision point is associated with a responsible actor.

### Role of AI Systems

The map clarifies whether AI systems provide analysis, suggestions,
classifications, or other forms of assistance.

Crucially, it distinguishes between **assistance and authority**.

### Escalation Pathways

Situations where automated outputs require human review are documented.

These escalation triggers ensure that unusual or high-risk cases receive
appropriate attention.

### Override Mechanisms

The map records how humans can intervene when automated outputs appear
incorrect or inappropriate.

### Responsibility Traceability

By documenting these elements, the map ensures that responsibility
remains visible within system workflows.

The Human--AI Boundary Map serves both as a design guide and as a
governance reference. It allows organisations to understand how
authority operates within complex systems.

# Risk and Misuse Register

The **Risk and Misuse Register** records foreseeable harms and
unintended consequences associated with a system.

Traditional risk management approaches often focus on technical
failures, such as system downtime or incorrect outputs. While these
concerns remain important, AI systems introduce additional forms of
risk.

These may include:

- biased outcomes affecting particular groups

- misuse of system outputs for unintended purposes

- over-reliance on automated recommendations

- erosion of professional expertise

- inequitable distribution of benefits or harms

The Risk and Misuse Register encourages designers to consider these
issues early in the design process.

The register typically includes several categories.

### Foreseeable Harm

Potential negative outcomes associated with system use.

### Risk Distribution

Identification of which individuals or groups may be affected by system
errors or misuse.

### Misuse Scenarios

Situations where system outputs could be used in ways that differ from
the intended purpose.

### Mitigation Strategies

Design features or governance mechanisms that reduce identified risks.

By documenting these considerations, the register encourages proactive
reflection on system impacts.

# Governance and Oversight Plan

The **Governance and Oversight Plan** describes how the system will
remain accountable once it becomes operational.

Many organisations produce governance policies but fail to embed
governance mechanisms into system design. As a result, oversight bodies
may struggle to understand or intervene in system behaviour.

The Governance and Oversight Plan addresses this problem by identifying
practical mechanisms that support governance.

Key components often include the following.

### Accountability Structures

Identification of individuals or teams responsible for system oversight.

### Audit Mechanisms

Description of logging, documentation, or traceability features that
enable system review.

### Contestability Procedures

Processes through which decisions influenced by the system can be
challenged or reconsidered.

### Scope Control

Mechanisms that prevent the system from expanding beyond its intended
domain without review.

The Governance and Oversight Plan ensures that systems remain visible to
those responsible for institutional accountability.

# Evaluation Log

The **Evaluation Log** records how the system performs over time.

Many AI systems are evaluated primarily through technical performance
metrics such as accuracy, precision, or response time. While these
measures are important, they do not capture the broader impacts of
systems on human capability and governance.

The Evaluation Log therefore includes multiple types of indicators.

### Capability Outcomes

Evidence that the system supports the intended capabilities described in
the System Capability Brief.

### Behavioural Indicators

Observations about how users interact with the system.

For example, the log may record whether users frequently override system
recommendations or whether they rely on automated outputs without
review.

### Governance Indicators

Information about system auditability, transparency, and oversight.

### Emerging Risks

New concerns identified during system operation.

Maintaining an Evaluation Log helps organisations detect capability
erosion, automation drift, or governance gaps before they become
entrenched.

# Retirement Notes

The final artefact in the toolkit addresses an often overlooked aspect
of system design: **how systems end**.

Many technologies remain in use long after their design assumptions are
outdated. As organisations become dependent on automated systems,
replacing or retiring them can become difficult.

The **Retirement Notes** document provides guidance for responsible
system decommissioning.

Key elements include:

### Conditions for Retirement

Circumstances under which the system should be replaced, redesigned, or
retired.

### Transition Planning

Strategies for transferring responsibilities to new systems or
processes.

### Data Preservation

Decisions about which system records should be archived for governance
or research purposes.

### Institutional Learning

Reflections on what the organisation learned from the system's
lifecycle.

By planning for system endings from the beginning, organisations avoid
becoming trapped by technologies that no longer serve their intended
purpose.

# Using the Toolkit

The CDD Design Artifacts Toolkit is intentionally lightweight.

These artefacts are not intended to slow development or create excessive
administrative burden. Instead, they provide structured checkpoints that
ensure responsibility remains visible throughout the system lifecycle.

In practice, organisations often adapt these artefacts to fit their
existing development processes.

For example, the System Capability Brief may be incorporated into
project initiation documents. Human--AI Boundary Maps may be integrated
into system architecture diagrams. Evaluation Logs may be connected to
operational monitoring dashboards.

The specific format is less important than the underlying goal: ensuring
that systems are designed, monitored, and evolved in ways that preserve
human capability and institutional accountability.

# Design Artifacts as Governance Infrastructure

Taken together, these artefacts represent more than documentation.

They form a governance infrastructure for AI systems.

By making capability intent, responsibility boundaries, risk
considerations, oversight mechanisms, and evaluation practices visible,
the toolkit ensures that system behaviour can be understood and governed
over time.

As artificial intelligence becomes more deeply embedded in institutional
processes, such infrastructure will become increasingly important.

Capability-Driven Development provides one approach to building that
infrastructure.

The CDD Design Artifacts Toolkit offers practical tools that
organisations can use to ensure that the systems they build remain not
only effective, but also accountable, transparent, and worthy of trust.

The design artefacts presented in this appendix provide conceptual
guidance.

Practical examples, evolving documentation, and future templates are
maintained in the Capability-Driven Development repository.

## Accessing the Capability-Driven Development Toolkit

The artefacts described in this appendix are maintained as part of the
**Capability-Driven Development repository**.

The repository contains:

- the CDD design method

- explanations of design artefacts

- architectural patterns

- applied system examples

- evolving guidance for responsible AI system design

Readers who wish to explore practical implementation guidance can access
the repository here:

https://github.com/cloudpedagogy/capability-driven-development

Over time, the repository may include:

- expanded artefact templates

- example implementations

- additional design patterns

- applied governance guidance

The repository is maintained as a **living resource**, allowing the
method to evolve as organisations apply Capability-Driven Development in
practice.
