# INFORMATIVE.md — Complete Professional Context for Harley Davidson Tobias

**Document purpose:** This is the source-of-truth context document for an AI assistant that will help improve Harley Davidson Tobias's portfolio website, resume, professional profile, project descriptions, and technical positioning.

**How to use this document:** Read this file before editing any portfolio content. It is intentionally much more detailed than a conventional portfolio page. Use it to understand the person and the engineering work behind the website, then turn the relevant information into concise, recruiter-friendly copy. Do not paste the entire document into the public website. The website should be selective; this document is the background reference.

**Accuracy rule:** Distinguish confirmed experience from experiments, prototypes, planned work, and information that needs verification. Do not invent dates, metrics, customer counts, production impact, formal certifications, ownership, or implementation details. Where this document says “verify,” inspect the source code, deployment records, certificate, project history, or ask Harley before making a public claim.

---

## 1. Professional identity

### Full name
**Harley Davidson Tobias**

### Recommended primary positioning
**AI Engineer & Software Engineer**

Alternative headline, depending on the page layout:

> Applied AI Engineer | LLM Applications, Workflow Orchestration, Android & Software Engineering

A concise value proposition:

> I build practical AI applications and software systems, combining a decade of software engineering experience with hands-on work in LLM integration, retrieval, agent workflows, cloud deployment, mobile engineering, APIs, and testing.

### Professional background
Harley has approximately **10+ years of software development experience**. His established background includes Android development, Kotlin, fintech/mobile applications, Huawei Mobile Services (HMS), API integration, web and backend-adjacent projects, and software quality/testing. His current professional direction is applied AI engineering: designing and integrating LLM-powered applications and the surrounding systems that make them useful.

His differentiator is not simply that he uses AI tools or writes prompts. He is approaching AI as a software systems problem: application architecture, context management, routing, workflow state, validation, retrieval, tool boundaries, backend integration, deployment, and human review.

### The central professional story
Harley is a software engineer extending an established engineering foundation into applied AI and LLM systems. His story should communicate a progression:

1. **Software engineering foundation:** Years of building and maintaining applications, especially Android and Huawei mobile systems, with API integration and testing.
2. **Applied AI experimentation:** Building local LLM applications and exploring retrieval-augmented generation (RAG), vector search, prompt construction, model selection, and AI-assisted coding workflows.
3. **Workflow and agent architecture:** Moving beyond a single prompt-to-model call toward explicit state, rules, routing, clarification, validation, and orchestration.
4. **Cloud integration and deployment:** Working with Dockerized applications, Amazon Elastic Container Registry (ECR), an EC2-hosted container environment, and Amazon Bedrock integration for LLM-backed application features. Describe the exact deployment ownership carefully; an AWS-focused colleague has been responsible for parts of the deployment process.
5. **Business-oriented AI applications:** Sharmaine is intended to apply LLM capabilities to practical business analysis, user-story preparation, QA planning, and chatbot workflows, with access to tools controlled through an MCP gateway where applicable.

### Best-fit professional categories
- Applied AI Engineer
- LLM Application Engineer
- AI Software Engineer
- Software Engineer, AI Products
- AI Workflow / Agent Systems Engineer
- Android Engineer / Android Developer
- Mobile Software Engineer
- API Integration and Quality Engineering

Do not present every category as a separate current job title. Lead with **AI Engineer & Software Engineer**, then show Android/mobile engineering as a proven foundation and LLM application engineering as the current specialization.

### Positioning boundaries
Use **applied AI / LLM application engineering** as the primary AI description. Do not imply that Harley is primarily a research scientist or a model-training specialist. He has experimented with local models and adapter/fine-tuning workflows, but portfolio claims should distinguish application-layer LLM engineering from foundational model research.

Avoid calling him an “Inference Engineer” as the sole or definitive title unless the portfolio is specifically tailored to that role and demonstrates sufficient evidence of inference serving, throughput/latency measurement, batching, quantization benchmarks, GPU optimization, and serving infrastructure. Inference engineering is a potential direction of growth, not a substitute for his more broadly supported current positioning.

---

## 2. How Harley approaches engineering

### Systems before prompts
A recurring architectural principle in Harley's AI work is that a reliable AI application should not be treated as only:

`Prompt → LLM → Answer`

His preferred mental model is closer to:

`Workflow State → Rules / Validation → Task Router → Clarification → Primary LLM → Validation / Evaluation → Result`

The exact sequence can vary by feature. The important idea is that the model is one component inside an application workflow, not the entire system.

### Key engineering principles
- **Explicit workflow state:** Track what the application is doing and what has already happened, rather than relying entirely on conversation history.
- **Rules and validation:** Use deterministic application rules to establish boundaries and validate required fields or outputs.
- **Routing:** Select an appropriate task path or model behavior based on the request rather than sending every request through the same expensive reasoning path.
- **Clarification:** Ask for missing required information before running a costly or consequential workflow.
- **Context management:** Supply relevant information to the model instead of indiscriminately adding all available context.
- **Structured output:** Use schemas or predictable output formats where downstream code needs to parse and act on a response.
- **Evaluation and repair:** Validate model output and handle failures instead of assuming a fluent response is a correct response.
- **Human-in-the-loop:** Preserve review and approval for work that needs human judgment, accountability, or business sign-off.
- **Security boundaries:** A retrieval result or an LLM response is not authorization. Permissions must be enforced by the application and tool gateway.
- **Budget awareness:** Consider token usage, model selection, tool calls, logging, and infrastructure costs as part of the system design.
- **Build and verify:** Use AI-assisted coding to learn and move faster, while still trying to understand, inspect, test, and validate the code and architecture.

These principles should be visible in the portfolio because they communicate engineering judgment rather than generic enthusiasm for AI.

---

## 3. Work history and established software engineering experience

### Android and fintech engineering
Harley has worked as an Android Developer in fintech, including work associated with TOP.ph / The Orange Platform. His mobile engineering background includes Android development and Huawei ecosystem integration. His salary and employment details are not relevant to public portfolio copy and should not be published unless he explicitly requests it.

Possible public summary:

> My software engineering foundation comes from building and supporting mobile applications, including fintech experiences across Android and Huawei ecosystems. That work taught me to think about integration, application behavior, maintainability, and the practical details that make software work outside a demo.

When describing TOP.ph or any employer product:
- Label it as **professional experience**, not as a personal product.
- State Harley's actual contribution (for example, feature development, API integration, maintenance, testing, or release support) only if confirmed by his work history or project evidence.
- Do not imply he independently built the entire fintech platform.
- Use public app listings only as references to the product, not as proof that he personally implemented every listed feature.

### Mobile and software development skills
The existing portfolio lists or implies skills across:
- Kotlin and Android development
- Huawei Mobile Services (HMS)
- API integration
- UI and application development
- Unit/integration testing tools and practices
- Web and full-stack project work
- SQL/data persistence and backend integration
- DevOps/cloud learning and implementation

The exact tools and proficiency level for each skill should be verified against the portfolio source, repositories, and Harley's actual usage. Avoid filling a skill list with every tool he has merely encountered.

---

## 4. Applied AI project: Clementine

### What Clementine is
**Clementine** is Harley's local-first personal AI assistant / LLM systems project. It has been a practical learning and experimentation environment for local language models, retrieval, application architecture, and assistant behavior. It is important to describe it as an evolving project with distinct phases, not as a single unchanged implementation.

### Evolution
The project history includes:
- Early local LLM experimentation using Ollama and a DeepSeek-R1-family model on an Apple Mac with an M2 Pro chip and 32 GB unified memory.
- A Python/FastAPI-oriented backend and vector-search/RAG experiments using Chroma and sentence embeddings (including an all-MiniLM-family embedding model).
- Work exploring identity/behavior shaping and adapter fine-tuning, including Mistral-family models and MLX-oriented experimentation.
- Later experimentation with Qwen-family instruction models on Apple Silicon, with attention to instruction following, reliability, coding assistance, and local inference.
- Workflow orchestration and application logic intended to reduce dependence on a single long prompt.

Do not imply every model or component was active at the same time. This is a project history spanning multiple experiments and revisions.

### Architecture concepts explored
- Local model inference
- FastAPI service layer
- Retrieval-augmented generation (RAG)
- Vector search / Chroma
- Embedding-based semantic retrieval
- Prompt and mode construction
- Workflow state
- Task routing
- Validation and evaluation
- Tool-call / streaming responses in parts of the application
- Modular agent roles and orchestration
- Epistemic Memory Engine (EME) concepts

### Workflow and agent concepts
Harley has described a multi-stage workflow and agent arrangement with roles such as:
- **Prompt Maker:** prepares or structures prompts for a task.
- **UserStoryAgent:** drafts user stories and related requirements.
- **SolutionsArchitectAgent:** reasons about technical structure and implementation approach.
- **SupervisorAgent:** coordinates the workflow and delegates or reviews work.
- **CodingAgent:** helps generate implementation code.
- **BugfixerAgent:** assists with debugging and corrections.

These are architectural roles/prototypes, not necessarily separate deployed autonomous services. Describe them as components or agent roles unless the code proves they run as independent agents.

### Epistemic Memory Engine (EME)
EME is an architectural concept intended to improve the relevance and organization of information supplied to an LLM. It is not a guarantee of perfect memory and does not “eliminate” irrelevant context or hallucination completely.

The intended idea is to select and structure useful knowledge, reduce unnecessary context, and provide relevant information to a reasoning workflow. The EME Council concept has also been considered in connection with model/API calls, including AWS Bedrock. When describing EME, use language such as “explores structured context selection and memory orchestration” rather than claiming 100% accuracy or perfect memory.

### Suitable public project description
**Clementine AI — Local LLM & AI Workflow Engineering**

> Clementine is my evolving local-first AI assistant project, where I explore LLM application architecture, retrieval-augmented generation, context management, and workflow orchestration. Across different iterations, I have experimented with local models, FastAPI-based services, vector search, prompt/mode routing, and validation-oriented workflows. The project reflects my interest in the engineering around an LLM—how context is selected, tasks are routed, outputs are checked, and assistant behavior is integrated into a useful application.

Suggested tags, only when accurate for the specific version shown:
`Python` · `FastAPI` · `LLMs` · `RAG` · `Chroma` · `Ollama` · `MLX` · `Workflow Orchestration`

### Status and claims
- Mark it as a **personal project / evolving prototype** unless a specific component is demonstrably used in production.
- Separate current working functionality from experiments and planned front ends.
- Do not claim “fully private” unless network access, telemetry, logging, storage, and data handling have been verified.
- Do not claim that RAG eliminates hallucinations.
- Do not imply the model itself was trained from scratch. If discussing adapters or fine-tuning, specify that this was model adaptation/experimentation, not foundational model pretraining.
- If describing a specific model version, include the actual version and hardware only if that information remains accurate for the current build.

---

## 5. Applied AI project: Sharmaine

### What Sharmaine is
**Sharmaine** is an AI application project conceived as a sister project to Clementine, with a stronger API-LLM / business-application direction. It is intended to turn LLM capabilities into a useful assistant for business analysis and quality engineering workflows, rather than simply being a general-purpose chat interface.

The use cases discussed include helping a user prepare:
- Technical and functional user stories
- Requirements and acceptance criteria
- QA integration-test plans and test cases
- Technical specifications and related structured artifacts
- Chatbot responses and, where enabled, controlled tool-assisted workflows

The project has been discussed with company leadership as a possible internal business capability. Describe its actual maturity accurately: proposal, prototype, pilot, integrated feature, or deployed service depending on what can be verified at the time of editing.

### Business workflow concept
The intended AI-assisted BA/QA workflow can be represented as:

`Discovery → Specification / User Stories → QA Planning → Review → Human Approval`

A multi-agent arrangement may use different roles for drafting, technical review, and QA. The value proposition is to help one user access several focused BA/QA capabilities, improve the speed of preparing structured artifacts, and maintain traceability from requirements to stories, acceptance criteria, and tests. It should not be presented as a fully autonomous replacement for human business analysts or QA engineers.

### API-based LLM architecture
The broad architecture is:

`User Interface → Sharmaine Backend → LLM Provider API`

The backend is the application boundary responsible for items such as authentication, sessions, guardrails, orchestration, prompt construction, context/RAG, and response handling. The LLM is an external service accessed through an API; it is not automatically running inside the Docker image just because the application is containerized.

When an MCP tool gateway is used, the architecture may extend to:

`User Interface → Sharmaine Backend / Orchestrator → Controlled MCP Gateway → Approved Tools / Data Sources`

MCP should be described as a controlled interface for tool access, not as the primary reasoning engine. The application and gateway should enforce authorization, allowed tools, input validation, and other security rules. RAG retrieves information; it does not itself grant permission to perform an action.

### AWS Bedrock integration — important portfolio evidence
Harley has worked on integrating **Amazon Bedrock** as an LLM provider for AI application/chatbot workflows associated with Sharmaine and related AI work. This is a distinct applied-AI integration achievement and should be explicitly represented in the portfolio if the implementation evidence is available.

The integration concept is:
1. The application receives a chat or workflow request.
2. Sharmaine's backend prepares the request, instructions, context, and any applicable workflow state.
3. The backend invokes a supported Bedrock model through the AWS SDK / Bedrock Runtime.
4. The application receives the model response and applies its own parsing, validation, and response handling.
5. If tools are enabled, application/gateway logic determines whether a tool can be called and validates its permissions and arguments; the model response alone must not authorize an action.

Implementation notes from the engineering discussions:
- Amazon Bedrock provides managed access to supported foundation models through AWS APIs.
- The model is accessed remotely; it is not embedded in the Docker container merely because the backend calls Bedrock.
- A Python backend may use the AWS SDK (`boto3`) and Bedrock Runtime APIs, subject to the actual implementation.
- For an AWS-hosted workload, IAM roles and least-privilege permissions are generally preferable to hard-coded long-lived access keys. Never publish keys, tokens, account IDs, secrets, or private deployment configuration.
- Model ID, AWS Region, IAM configuration, API method, streaming behavior, and the precise state of the integration must be confirmed from the source code and deployment configuration before publishing exact technical claims.
- Do not state that all Sharmaine agents use Bedrock, or that the whole system is production-ready, unless the current implementation proves it.

### Safe public description
**Sharmaine — AI-Assisted BA/QA Workflows & LLM Integration**

> Sharmaine is an AI application project focused on bringing LLM capabilities into practical business-analysis and QA workflows, including user-story drafting, acceptance criteria, and test planning. I have worked on API-based LLM integration, including Amazon Bedrock, and on structuring the application around workflow orchestration and controlled tool access. The goal is to make generated artifacts easier to review and use within an engineering process, with human approval retained for important decisions.

Suggested tags, after verifying the code:
`Python` · `LLM API Integration` · `Amazon Bedrock` · `AWS SDK / boto3` · `Docker` · `MCP` · `Workflow Orchestration` · `QA Automation Support`

### Do not overstate
- Do not say Sharmaine autonomously replaces a BA, QA engineer, or team.
- Do not claim measurable time savings without a measured pilot.
- Do not state that every MCP tool is secure simply because MCP is used; describe the actual controls implemented.
- Do not claim a production deployment if the project is still in prototype/pilot stage.
- Do not conflate the business case, proposed architecture, and already implemented features.
- Confirm whether the Bedrock integration is currently working in a live environment, a test environment, or development before choosing a status label.

---

## 6. Docker and AWS deployment experience — explicitly include this

This section is important and was not explicit enough in the earlier portfolio specification.

### What should be represented
Harley has worked with Dockerized AI application deployment and the AWS container workflow involving **Amazon Elastic Container Registry (ECR)** and an **Amazon EC2-hosted environment**. The project has been described as an application image stored in ECR and running as a Docker container on EC2. An AWS-focused colleague has handled or supported parts of the deployment process, so the public wording must be honest about which deployment steps Harley personally performed versus collaborated on or learned from.

Do not erase this experience from the portfolio simply because another colleague managed some infrastructure. At the same time, do not imply sole ownership of AWS infrastructure if that is not true.

### Relevant concepts in the workflow
A typical container delivery path for this kind of application is:

1. Package the backend/application into a Docker image.
2. Build and tag the image.
3. Push the image to Amazon ECR, which stores container images.
4. Run or update the container on an AWS compute environment such as EC2.
5. Configure environment-specific settings, networking, logging, and runtime permissions.
6. Have the application call Amazon Bedrock or another external service through its API.
7. Verify that the container starts correctly, the service is reachable, and required integrations work.

This is a conceptual sequence. The AI editing the portfolio must not assume Harley personally performed every step unless supported by his work or repository/deployment evidence.

### How Docker, ECR, EC2, and Bedrock relate
- **Docker:** packages the application and its runtime dependencies into a container image.
- **Amazon ECR:** stores the image so the deployment environment can retrieve it.
- **Amazon EC2:** provides compute capacity on which a Docker container can run. Confirm the exact runtime arrangement before naming additional services such as ECS or Fargate.
- **Amazon Bedrock:** provides model inference through an API. The LLM is accessed remotely; it does not have to be installed inside the container.
- **IAM:** controls AWS access. Prefer scoped roles and least privilege for hosted workloads; do not place credentials in source code or a Docker image.
- **Configuration/secrets:** keep region, model identifiers, and credentials outside public code. Do not publish secrets or sensitive infrastructure details.

### Recommended portfolio project/case-study entry
**Sharmaine — Containerized AI Application & Amazon Bedrock Integration**

**One-line summary:**
> Worked on containerized deployment and AWS LLM integration for an AI application, connecting a Docker-based backend workflow with Amazon ECR/EC2 and Amazon Bedrock.

**Expanded description:**
> I have worked on packaging an AI application for containerized deployment using Docker, with the container image stored in Amazon ECR and the application running in an EC2-hosted environment. I also worked on integrating Amazon Bedrock as an API-based LLM capability for chatbot/workflow functionality. This work connects application-layer AI engineering with cloud deployment concepts: the application runs in a container, while model inference is provided through an AWS-managed API. Parts of the deployment process involved collaboration with an AWS-focused colleague, so the project description should accurately distinguish my implementation work from shared infrastructure responsibilities.

Use this wording only after confirming that the current source/deployment state supports each sentence. If Harley personally built and pushed the Docker image, say that. If he configured the ECR repository, say that only if verified. If a colleague performed the push/deployment, use “worked with,” “contributed to,” or “collaborated on” instead of “independently deployed.”

### Suggested skill labels
Use a meaningful, accurate selection:
- `Docker`
- `Amazon ECR`
- `Amazon EC2`
- `Amazon Bedrock`
- `LLM API Integration`
- `AWS IAM` (only if Harley has hands-on configuration knowledge)
- `Python / FastAPI` (only if the actual backend uses them)
- `Containerized Application Deployment`

Do not add `Kubernetes`, `ECS`, `Fargate`, `Terraform`, `CI/CD`, or production-scale infrastructure engineering unless Harley has actually used them and can discuss the implementation.

### Strong technical framing
This is useful evidence that Harley is not only experimenting with local models. He is learning to connect an AI application to managed model APIs and a cloud-hosted container environment. The public portfolio should frame this as **applied LLM integration and containerized cloud deployment experience**, not as proof of mastery of all AWS architecture.

---

## 7. Other portfolio projects currently represented

The existing portfolio contains a selection of professional, client, personal, and historical projects. Each must be labeled according to its real ownership and status.

### Digital Bingo Game System
**Potential category:** Full-Stack Web Application · Real-Time Event Workflow

Current portfolio context describes a web-based bingo system with registration, draw display, moderator verification, and public display components. The listed stack includes React and Node.js. Confirm the exact implementation and deployment.

Suggested description:

> A web-based event workflow supporting participant registration, live draw display, moderator verification, and a public-facing number board. The project demonstrates full-stack application thinking and coordination between participant, host, and display interfaces.

Do not claim event scale, uptime, or reliability numbers without evidence. Choose the correct status label (personal, client, community, or professional project).

### MyTianggePH
**Potential category:** Mobile Application · Marketplace

The current portfolio lists this as a marketplace-oriented project. Confirm the platform, exact contribution, technology stack, and whether it was professional or independent work.

Suggested description, only after validation:

> Marketplace application work focused on connecting customers with Filipino products and services. The project entry should identify my specific contribution and the platform or features I worked on.

### Servicio International
**Potential category:** Service Platform · Web / Mobile (verify)

The current portfolio associates this name with service operations, including hospitality and maintenance. Confirm what was actually built, the technology stack, and Harley's role.

### PopsicleMag
**Potential category:** Digital Media · Web

The current portfolio associates this project with digital media/publication content around culture, art, fashion, and lifestyle. Confirm whether Harley worked on frontend development, a CMS, site maintenance, or another specific area before publishing technical details.

### Giordano Philippines
**Potential category:** Retail Technology · POS

The current portfolio associates this experience with retail point-of-sale systems. Describe the actual role and responsibilities. Do not imply ownership of the entire retail/POS platform.

### New Era Philippines
**Potential category:** Retail Technology · POS

The current portfolio associates this experience with retail point-of-sale systems. Confirm the timeframe, exact responsibilities, and stack before making specific claims.

### Event Registration System
**Potential category:** Web Application · Event Registration

The current portfolio describes an event registration experience that includes a personalized video tribute component. Confirm the implementation details and exact contribution. Do not publish private attendee information, personal media, or private event data without permission.

### TOP.ph / The Orange Platform
**Potential category:** Fintech · Android · Huawei HMS

This is professional experience, not automatically a personal project. Describe Harley's actual contribution to the mobile application, such as feature implementation, integration, maintenance, or testing, only where verified. Confirm which public links and screenshots are appropriate to show.

### Portfolio project order
Recommended order for the current career direction:
1. **Sharmaine** — business-focused AI workflow and Bedrock integration, if the implementation is sufficiently demonstrable.
2. **Clementine AI** — local LLM, RAG, context management, and workflow engineering.
3. **Docker + AWS deployment case study** — may be a separate case study or part of Sharmaine, depending on what can be shown without duplicating content.
4. **TOP.ph / fintech mobile engineering** — established professional experience.
5. **Digital Bingo Game System** — full-stack system work.
6. Other verified projects, ordered by relevance and evidence.

If Sharmaine's cloud integration is not yet stable or public-safe, present it as a prototype or engineering case study rather than implying production maturity. Do not force every historical project to have equal visual prominence.

---

## 8. Skills taxonomy for the website

The skill section should be organized around engineering capabilities rather than a large, undifferentiated list.

### A. Applied AI & LLM Systems
Potential skills:
- LLM application development
- API-based LLM integration
- Prompt construction and structured output
- Retrieval-augmented generation (RAG)
- Embeddings and semantic search
- Vector storage / Chroma
- Local LLM experimentation
- Model selection and inference experimentation
- Workflow orchestration
- Context and memory management
- Validation-oriented AI workflows
- Multi-role / multi-agent workflow prototyping
- Human-in-the-loop review

Use these labels only to the degree that the portfolio's code and demos support them. “LLM application engineering” is safer and more accurate than implying foundational-model research expertise.

### B. Cloud & Containerization
Potential skills:
- Docker
- Amazon Elastic Container Registry (ECR)
- Amazon EC2
- Amazon Bedrock
- AWS SDK / `boto3` (if used in code)
- IAM concepts / least-privilege access (claim hands-on configuration only if verified)
- Cloud-hosted LLM API integration

Be precise about whether the experience is hands-on implementation, collaborative deployment, or learning/prototyping.

### C. Android & Mobile Engineering
Potential skills:
- Kotlin
- Android development
- Android application architecture
- Huawei Mobile Services (HMS)
- Mobile API integration
- Application maintenance and debugging
- Mobile testing

Only list specific libraries or architecture patterns—such as Jetpack Compose, MVVM, Hilt, Espresso, Mockito, or JUnit—if they are still accurate and relevant to the work shown.

### D. Backend & Web Engineering
Potential skills from existing project context:
- Python
- FastAPI
- REST API integration
- React
- Node.js
- HTML/CSS/JavaScript
- Service integration
- Application-level orchestration

Verify the technologies per project; not every listed skill necessarily applies to every project.

### E. Quality Engineering & Testing
Potential skills:
- API testing
- Unit testing
- Integration testing
- Test-case design
- Validation and error-path testing
- QA planning support
- Structured acceptance criteria
- AI-assisted test preparation

Do not imply full automated QA coverage or production-grade test infrastructure without evidence. If tools such as Postman, Espresso, Mockito, or JUnit are included, confirm the exact usage.

### F. Data & Retrieval
Potential skills:
- SQL / SQLite (if applicable to the current work)
- Chroma
- Embeddings
- Semantic retrieval
- Data modeling and persistence
- Context selection and organization

Keep database administration separate from application-level use of a database.

### Proficiency labels
If the website displays levels, avoid arbitrary percentages such as “95% mastery.” Use honest categories instead:
- **Professional experience**
- **Hands-on project experience**
- **Working knowledge**
- **Currently exploring**

A skill should be listed because Harley can explain or demonstrate it, not because it appeared in a tutorial or was suggested by an AI assistant.

---

## 9. About-me copy for the public website

### Recommended full About section

> I’m Harley Davidson Tobias, a software engineer with more than a decade of experience across mobile applications, API integrations, testing, and software delivery. My foundation is in Android development and Huawei mobile ecosystems, including work in fintech.
>
> My current focus is applied AI engineering: building LLM-powered applications and connecting them to real workflows. Through projects such as Clementine and Sharmaine, I explore local model inference, retrieval-augmented generation, context management, workflow orchestration, and API-based model integration—including Amazon Bedrock.
>
> I’m interested in the engineering around the model: how an application selects relevant context, routes a task, validates an output, controls tool access, and gives a human the right point to review the result. I have also worked with Dockerized applications and AWS container workflows involving ECR and EC2-hosted execution.
>
> I learn by building, inspecting, and testing systems. I use AI-assisted development to accelerate experimentation, while treating architecture, validation, security boundaries, and clear technical understanding as essential parts of the work.
>
> I’m looking to contribute to teams turning AI capabilities into practical, dependable software—bringing together my existing software engineering experience and my growing specialization in LLM application systems.

This copy is a draft, not a claim that every described component is in production. Adjust the wording to reflect the current state of each project.

### Short About version
> Software engineer with 10+ years of experience in mobile development, APIs, and software testing, now focused on applied AI and LLM applications. I build and experiment with AI workflows, retrieval and context systems, Amazon Bedrock integrations, and Dockerized applications running in AWS environments.

### Short professional bio
> Harley Davidson Tobias is a software engineer focused on applied AI and LLM application development, with a background in Android, Huawei mobile engineering, API integration, and testing. His projects explore local LLM systems, workflow orchestration, retrieval, Amazon Bedrock integration, and containerized cloud deployment.

---

## 10. Hero section and headline

### Recommended headline
**I build AI systems that solve real engineering problems.**

### Eyebrow
`APPLIED AI · SOFTWARE ENGINEERING · MOBILE SYSTEMS`

### Supporting copy
> I’m a software engineer with 10+ years of experience across mobile applications, APIs, and software testing. Today, I focus on LLM-powered applications, workflow orchestration, and cloud integration—connecting AI capabilities to software systems that can be tested, reviewed, and used.

### Role rotation
Recommended order:
1. `AI Engineer`
2. `LLM Application Engineer`
3. `Software Engineer`
4. `Android & Huawei Developer`
5. `AI Workflow Engineer`

Avoid cycling through so many labels that the visitor cannot identify the main professional identity. Keep **AI Engineer & Software Engineer** as the stable identity; use the rotating line as supporting context.

### Primary CTA
`Explore Selected Work`

### Secondary CTA
`Contact Me`

### Optional third action
`View GitHub` or `View Resume`, but only if the destination exists and is current.

---

## 11. Portfolio navigation and section labels

The existing site has a stylized, sci-fi, game-inspired interface, including a system/terminal motif, project “missions,” a skill tree, progress/achievement indicators, and interactive contact reveal.

Keep the personality, but make the site's purpose immediately clear to a recruiter, engineering manager, or prospective collaborator.

| Existing concept / label | Recommended label |
|---|---|
| `HDT.OS` / `HDT.os` | `HARLEY.TOBIAS` or `HT // ENGINEERING` |
| `Missions completed` | `Selected Work` |
| `Skill tree` | `Technical Expertise` |
| `AWS certificates` | `Learning & Certifications` |
| `Ready to start a new run?` | `Have a technical problem worth solving?` |
| `See my work` | `Explore Selected Work` |
| `Open the terminal` | `Explore Interactive Portfolio` |
| `Open` on a project card | `View Project` |
| `Client:` | `Organization / Context:` |
| `Start` in skill navigation | `Overview` |
| `AI` in skill navigation | `Applied AI` |
| `LV 1` | `PROFILE`, or retain only as decoration |
| `Achievements 0/6` | `Portfolio discoveries 0/6`, or remove if distracting |
| Hold-to-reveal contact interaction | A direct visible `Contact Me` action, with the animation optional |

The site should not require a visitor to discover Easter eggs, complete an interaction, or operate a terminal to find core experience, contact information, or project links.

---

## 12. Learning and certifications

The current website presents AWS learning certificates / course certificates. Label this section accurately.

Recommended title:
**Learning & Certifications**

Suggested description:
> Selected AWS learning certificates and technical training supporting my continued development in cloud and AI engineering.

Important distinction:
- A course completion certificate or learning badge is not necessarily the same as an official AWS Certification exam credential.
- Do not label a course certificate as “AWS Certified” unless Harley holds the corresponding official certification.
- Verify the exact number of displayed certificates and ensure each badge links to the correct certificate.
- If there are 14 learning certificates, use that number only while the list remains accurate.

---

## 13. Interactive terminal / portfolio assistant

The existing portfolio includes a scripted interactive terminal experience. The interface can remain as a personality feature, but its behavior must be represented truthfully.

- If the terminal uses predefined responses, label it as an **interactive portfolio demo** or **scripted terminal**.
- Do not call it a live AI chatbot unless it actually calls a model at runtime.
- Do not imply the terminal can access private repositories, run commands, query live systems, or perform real operations unless those capabilities exist and are safe to expose.
- Provide ordinary navigation and visible links so the terminal is optional.
- If a live LLM is added later, document its actual data access, limitations, and privacy behavior.

Possible description:
> An interactive, scripted portfolio terminal for exploring selected projects and skills.

---

## 14. Privacy, security, and public information

The public portfolio must not disclose:
- API keys, tokens, passwords, credentials, or environment files
- AWS account identifiers or private endpoints unless intentionally approved for public use
- Internal source code, private architecture diagrams, customer data, or internal fintech information
- Private user stories, real customer information, or company-sensitive prompts
- Private event attendee information or personal media without permission
- Non-public employer data, internal metrics, or confidential project details

When discussing AI systems, avoid claiming “fully private,” “zero data retention,” “secure by design,” or “compliant” unless those claims have been independently verified and are safe to publish. It is fine to discuss principles such as least privilege, validation, and human review as design goals; distinguish goals from implemented controls.

For cloud deployments, show architecture at a useful high level without revealing credentials, private IPs, secrets, account IDs, or security-sensitive details.

---

## 15. Project maturity and evidence labels

Every project should have a visible status label. Select one that reflects the current evidence:

- **Professional experience** — work performed in an employment context.
- **Personal project** — independently developed project.
- **Prototype** — working experiment or early implementation.
- **In development** — actively being built.
- **Pilot** — limited real-world trial; use only if an actual pilot has started.
- **Deployed** — deployed to a real environment; specify whether development, staging, or production if useful and safe.
- **Planned** — not yet implemented.
- **Learning / exploration** — tested or studied but not integrated into a durable project.

Do not use “production-ready” as a synonym for “it runs.” Production readiness implies appropriate reliability, security, monitoring, deployment practices, support, and operational validation.

For every project card, aim to include:
1. Name
2. Category
3. Problem or use case
4. Harley's contribution
5. Technologies actually used
6. Current status
7. Evidence: repository, demo, screenshots, public listing, or technical write-up where available
8. Limitations or next steps if the project is a prototype

---

## 16. Resume and career narrative

### Suggested resume summary
> Applied AI and software engineer with 10+ years of software development experience across Android/mobile applications, API integration, and testing. Building LLM-powered applications and workflows involving local model experimentation, RAG, context management, model/API integration, Amazon Bedrock, and Dockerized deployment in AWS environments. Focused on connecting AI capabilities to structured workflows with validation, controlled tool access, and human review.

Before using this summary in a resume, verify which AWS and AI components were implemented hands-on and which were collaborative or exploratory. Adjust the phrasing to reflect actual contribution.

### Suggested LinkedIn headline
> AI Engineer | LLM Applications & Workflow Orchestration | Android / Huawei Software Engineering | AWS Bedrock & Docker

A more conservative alternative if the Bedrock deployment is still a prototype:
> Software Engineer Moving into Applied AI | LLM Applications, RAG & Workflow Orchestration | Android / Huawei | AWS Exploration

### Career direction
Harley's current trajectory is toward applied AI engineering and LLM application systems, using his existing software engineering background as the foundation. The portfolio should support roles involving:
- LLM API integration and application development
- AI workflow orchestration
- RAG and context/retrieval systems
- Internal AI tools and productivity applications
- AI-assisted BA/QA workflow tools
- Containerized application integration and cloud deployment
- Mobile engineering roles that benefit from AI integration experience

The site should not overfocus on every new AI term. Concrete project descriptions, architecture decisions, testing, and evidence are stronger than a long list of buzzwords.

---

## 17. Implementation instructions for the AI editing the website

### First: inspect the current site
Use the current `indexv2.html` as the baseline. Identify its existing sections, project data, navigation, animations, interactions, and external links before making changes. Preserve the existing design system unless there is a clear reason to change it.

### Second: update content without inventing facts
- Replace vague or game-only section labels with clear professional labels.
- Add or improve the About section.
- Rework the hero headline, supporting copy, and calls to action.
- Give Sharmaine and Clementine prominent, accurate case studies.
- Explicitly represent Docker, ECR/EC2, and Bedrock work where supported.
- Organize skills by capability and experience area.
- Clarify project ownership and maturity.
- Keep the interactive style as a visual signature, not as a barrier to information.
- Preserve working links and verify all updated destinations.

### Third: check the implementation
- Do not break the current layout, animations, responsive behavior, or interactive elements.
- Check mobile and desktop layouts.
- Ensure text remains readable and accessible.
- Provide a visible way to reach contact information.
- Check keyboard navigation and focus states.
- Avoid relying only on color, animation, or hover for important information.
- Ensure every project modal/card has a clear close/open path and works on touch devices.
- Confirm that external links open the correct destination.
- Do not insert secret values, private internal data, or unverified metrics.

### Fourth: report uncertainty
If a fact is not supported by the HTML, source repository, or this document, do not silently invent it. Keep the existing wording temporarily or flag the item for Harley to confirm. In particular, verify:
- Harley's exact role and contributions on each project
- Which Sharmaine features are implemented versus proposed
- The current status of the Bedrock integration
- Which Docker/ECR/EC2 deployment steps Harley personally performed
- Exact project technology stacks
- The status and links for public demos/repositories
- Exact AWS course/certificate titles and credential type
- Whether any project can be publicly shown without confidentiality concerns

### Fifth: return useful deliverables
After editing, report:
1. What sections and labels changed
2. What project descriptions were added or rewritten
3. How Sharmaine's Bedrock and Docker/ECR/EC2 experience was represented
4. Any claims that still need Harley's confirmation
5. Any links or interactions that need manual verification

---

## 18. Priority order for the portfolio

### Priority 1 — Immediate
1. Make the professional identity clear within the first screen.
2. Add a concise but informative About section.
3. Make Sharmaine and Clementine visible as the two main AI case studies.
4. Explicitly document Bedrock integration and Docker/ECR/EC2 work, with honest attribution.
5. Make contact and project navigation obvious without requiring an Easter egg.
6. Ensure the terminal is described accurately if it is scripted.

### Priority 2 — Credibility
1. Clarify the problem, contribution, stack, and status for each project.
2. Separate professional experience from personal/client projects.
3. Replace unverified skill levels with honest proficiency categories.
4. Distinguish AWS learning certificates from official AWS Certifications.
5. Add architecture diagrams or short technical write-ups only where they reflect the actual implementation and contain no confidential information.

### Priority 3 — Polish
1. Refine animation timing and reduced-motion behavior.
2. Improve keyboard and touch accessibility.
3. Standardize project card structure and technical labels.
4. Make responsive layout and typography consistent.
5. Keep the sci-fi theme but reduce jargon where it interferes with clarity.

---

## 19. Final writing principles

The public portfolio should communicate these five things quickly:

1. **Who Harley is:** an AI Engineer & Software Engineer with a decade-plus software background.
2. **What he builds:** practical LLM applications, workflows, integrations, and mobile/software systems.
3. **What makes his approach distinctive:** he thinks about state, context, routing, validation, tool permissions, testing, and human review—not only prompts.
4. **What he has worked with:** local LLM/RAG experiments, Sharmaine's API-based LLM workflows, Amazon Bedrock integration, and Dockerized AWS container workflows involving ECR and EC2, with exact ownership represented honestly.
5. **What the visitor should do next:** inspect a project, view evidence, contact him, or review his resume.

### Voice and tone
- Confident, grounded, technical, and human.
- Prefer concrete verbs: built, integrated, tested, designed, prototyped, deployed, collaborated, evaluated.
- Use “worked on” or “contributed to” when ownership was shared.
- Explain acronyms on first use when a broad audience may not know them.
- Do not describe AI-assisted coding as cheating. Emphasize learning, implementation, inspection, and verification.
- Avoid exaggerated claims such as “revolutionary,” “fully autonomous,” “zero hallucinations,” “perfect memory,” or “enterprise-grade” without evidence.
- Avoid presenting exploratory skills as professional mastery.
- Keep the public page concise. Use this file as context, not as the page's entire copy.

---

## 20. Important final note to the AI editor

This file is a detailed working brief, not proof that every listed component is currently live or production-ready. It combines the current portfolio context with information about Harley's project history and stated work. Some details—especially exact contributions, deployment ownership, and current integration status—must be confirmed before being converted into definitive public claims.

The most important improvement is to represent Harley as a software engineer who is actively building applied AI systems and connecting them to real application and cloud workflows. **Do not omit the Amazon Bedrock chatbot integration or the Docker/ECR/EC2 deployment experience**, but describe the work at the level the evidence supports. Preserve the existing site's visual identity while making the professional value immediately understandable.
