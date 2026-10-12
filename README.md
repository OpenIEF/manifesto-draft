# The Interoperable Environment Framework

## A Manifesto for Open Interoperability Across Physical and Digital Environments

---

## 1. The Moment

Buildings, factories, transport systems, logistics facilities, and public infrastructure are becoming shared physical and digital environments. Devices, robots, machines, software services, and human operators increasingly depend on one another.

A production process may span equipment, scheduling software, and human decisions. Access through a building may depend on doors, elevators, digital credentials, and changing operating conditions. These relationships matter as much as the capabilities of any individual system.

Yet systems are still commonly developed as separate ecosystems, with different representations of identity, capability, state, intent, and permission. Each new combination demands another integration.

As environments become more connected and autonomous, this fragmentation becomes a structural limit on scale.

**Interoperability must become foundational.**

---

## 2. The Problem

Connectivity allows systems to exchange messages. It does not ensure that they understand those messages, agree on permitted actions, or know what outcomes to expect.

A door can report its state without describing which spaces it connects. An elevator can acknowledge a request without confirming a reservation. A map can describe a route without reflecting a temporary closure.

Interoperability requires shared meaning and agreed behaviour. Participants need common ways to describe their capabilities, state, intent, and requirements, alongside the resources, relationships, constraints, and permissions that shape their interactions.

Without these foundations, each deployment becomes another integration exercise. Fragmentation increases cost, slows adoption, creates vendor dependency, and weakens long-term infrastructure investment.

The problem is not confined to robots, devices, or platforms. It is interoperability across the environment itself.

---

## 3. The Principle

The Interoperable Environment Framework (IEF) treats shared semantic models and interaction contracts as common infrastructure.

**The environment is the organising context. No class of participant is the centre of the Framework.**

IEF must describe both the systems that participate and the spaces, resources, services, and relationships through which they operate. A shared environment must remain meaningful regardless of which robots, devices, or platforms are present.

These foundations must be open, vendor-neutral, transparently specified, machine-readable, durable across technology cycles, and grounded in real deployments. No single manufacturer, platform provider, or AI ecosystem should control them.

Shared contracts allow diverse systems to work together without requiring common internal architectures. They support safety, scalability, and infrastructure stability while enabling competition through capability and service rather than control of integration pathways.

Shared meaning does not imply centralised operational control. System owners and operators retain authority over their systems, resources, and access policies.

**The Framework must be understandable by humans and machines.**

Participants should be able to use AI systems, including large language models (LLMs), to interpret IEF specifications, map existing systems into them, develop adapters, and identify implementation gaps.

AI assists adoption. It is neither a prerequisite for interoperability nor the authority on conformance. Explicit, versioned specifications remain the basis for implementation and validation.

---

## 4. The Commitment

The Interoperable Environment Framework exists to define and steward open interoperability standards for systems operating across physical and digital environments.

It does not replace existing middleware, platforms, or deployment architectures. It defines the interoperability contracts that allow them to coexist.

The Framework is committed to:

- Transparent and structured specification development
- Vendor-neutral technical foundations
- Middleware independence
- Durable semantic and coordination models
- Validation through real-world deployment
- Public accessibility of core specifications

Interoperability must be practical, implementable, and capable of long-term evolution.

---

## 5. The Structure

IEF distinguishes **four architectural layers** from **six complementary specification areas**.

The layers organise the work from shared meaning to working implementations. The specification areas address participants, the environment itself, and the trust requirements that apply across both.

### Specification Areas

| Specification area | Focus | Contribution to a shared environment |
|---|---|---|
| **IEF Infrastructure** | Shared facilities, resources, operating conditions, and constraints | Makes the environment more than a collection of devices by describing shared capabilities, resource availability, and site-wide conditions. |
| **IEF Spatial** | Places, zones, connectivity, and spatial relationships | Gives participants a common way to describe where things are, how spaces connect, and where conditions or restrictions apply. |
| **IEF Robot** | Robotic participants, including their capabilities, state, intent, and actions | Allows robots to participate in a shared environment without making their requirements the organising model for every other system. |
| **IEF Device** | Physical devices, machines, sensors, and equipment | Makes physical capabilities discoverable and usable through common descriptions and interaction contracts. |
| **IEF Digital Service** | Software services, platforms, and software agents | Allows non-physical capabilities, such as booking, work-order management, and orchestration, to participate directly rather than being forced into a device model. |
| **IEF Security** | Identity, authentication, authorisation, and trust | Establishes common requirements for who may participate, what they may access, and which actions they may request. |

Infrastructure and Spatial primarily describe the environment. Robot, Device, and Digital Service primarily describe participants. Security applies across both.

These areas are complementary, not mutually exclusive categories or additional layers. A building platform may expose digital services, manage infrastructure, and publish spatial information. Each area can contribute definitions, interaction contracts, conformance requirements, and implementation artefacts through the same four-layer architecture.

A corridor closure, for example, should have the same meaning for a robot, a maintenance team, and a scheduling service. It remains relevant even when no robot is present.

### Semantic Layer

Defines what concepts mean, independently of how they are transported or implemented.

The shared model covers identity, capabilities, state, intent, actions, events, resources, services, spaces, relationships, constraints, and permissions. It distinguishes participants that act from the places and resources they use or manage. A space can be represented without being treated as an actor.

Definitions should provide stable identifiers, explicit relationships, constraints, and examples in aligned human-readable and machine-readable forms. Common concepts should be reused across specification areas rather than redefined independently.

Mappings to existing standards should be explicit and versioned, with gaps and ambiguities recorded rather than silently approximated.

### Interoperability Layer

Defines how participants discover capabilities, exchange state and intent, request actions, reserve resources, and coordinate with one another or with services representing the environment.

Interaction contracts describe preconditions, requests, responses, outcomes, and failure behaviour. They distinguish a request from permission to act, acknowledgement from completion, and reported state from a guarantee of future availability.

Contracts remain independent of any single middleware or transport. Protocol-specific bindings and mappings make them implementable across different technology stacks.

IEF interactions must be authenticated and governed by explicit authorisation policies. Open specifications do not imply unrestricted access.

Schemas, interface descriptions, examples, and mappings should support conventional tooling and AI-assisted integration. An adapter must preserve the required meaning and behaviour, not merely translate fields.

### Conformance Layer

Defines how implementations demonstrate that they meet specified requirements.

Conformance declarations identify the specifications or profiles, versions, and capabilities supported. Conformance classes distinguish required and optional behaviour, while validation establishes compatibility within the declared scope.

Conformance can cover participants, environmental representations, and the adapters that connect existing systems to IEF. An implementation need not support every specification area, but remains subject to the common requirements applicable to its interactions.

Validation must address behaviour as well as data structure. Schema validity alone does not establish conformance. Claims must be supported by the evidence required by the relevant specification.

AI may assist gap analysis and test preparation. It does not determine whether an implementation conforms.

### Implementation Layer

Covers the systems and artefacts that realise IEF contracts, including native implementations, adapters, gateways, reference software, and test tools.

Robots, equipment, building systems, spatial databases, digital twins, and software platforms may participate through existing architectures, provided their exposed interfaces and behaviour meet the relevant contracts.

AI-assisted adoption should support a practical workflow: interpret existing documentation and interfaces, propose explicit mappings to IEF, generate adapter scaffolding or configuration, and validate the result against the applicable requirements.

Generated mappings should identify assumptions, gaps, and unsupported capabilities. AI-generated code, tests, and documentation remain subject to the same review and validation as manually produced work.

AI agents operating within an environment are themselves participants, subject to the same security and conformance requirements as other systems.

### Consistency Across Layers

Each release should identify its authoritative normative material and distinguish it from guidance and examples. Human-readable specifications and machine-readable artefacts should remain aligned through shared identifiers, explicit versions, and traceable links between concepts, contracts, mappings, and tests.

Changes must be reviewed across dependent specifications so that the layers evolve coherently.

The Framework defines shared contracts, not a central platform or execution environment.

---

## 6. Governance

The Interoperable Environment Framework is developed and stewarded through an open, vendor-neutral consortium.

The consortium brings together stakeholders to define and maintain open interoperability specifications for physical and digital environments.

Governance is organised through formally chartered working groups responsible for defined technical domains. Each working group operates under publicly documented procedures, including:

- Transparent proposal submission
- Public review periods
- Recorded deliberation
- Consensus-based decision processes
- Versioned specification release cycles

Specifications progress through defined maturity stages, with clear distinction between draft, candidate, and stable releases. Revisions are documented, traceable, and subject to structured review.

Participation is open to commercial entities that see a fit between their work and IEF, and to public authorities responsible for deployment, operation, integration, or regulation of systems. Decision-making structures are designed to preserve vendor neutrality and prevent dominance by any single organisation or market segment.

The consortium maintains:

- Clear intellectual property policies
- Open access to core specifications
- Public archives of technical discussions
- Defined mechanisms for implementation feedback

The role of governance is not to control implementations. It is to steward shared technical foundations that enable interoperable ecosystems to evolve predictably over time.

Accountability rests with those responsible for systems operating in real environments. Stewardship responsibility rests with the consortium as a whole.

---

## 7. The Invitation

We invite participation from:

- Robotics manufacturers
- Device and equipment manufacturers
- Software, middleware, and platform providers
- Fleet operators
- Infrastructure owners and integrators
- Building and city system operators
- Industrial system operators
- Public authorities and regulators responsible for safety and infrastructure

This list is not exhaustive. **Any commercial entity that sees a fit between its work and IEF is welcome to join and contribute.** Participation is not limited to a particular industry, technology, or stage of adoption.

The Framework is built for real deployments and real environments. Its specifications are shaped by implementation experience, operational constraints, and regulatory responsibility.

It is not an academic consortium or a theoretical forum. Membership is not open to academic institutions or individuals participating in an academic capacity.

Interconnected physical and digital systems are becoming part of critical infrastructure. The foundations that enable them to interoperate must reflect that responsibility.

Interoperability must be built by those who deploy, operate, integrate, and regulate systems at scale.
