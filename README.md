[![awseome-cedar.png](https://i.postimg.cc/Kz4gVS6Y/awseome-cedar.png)](https://postimg.cc/wy8vyPTK)

# Cedar Awesome [![Awesome](https://awesome.re/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of awesome tools, libraries, articles and research for [Cedar](https://cedarpolicy.com/), the open source policy language for fine-grained authorization.

Cedar lets you express authorization rules as readable policies, decouple them from application code, and reason about them automatically. It is a CNCF Sandbox project, and powers Amazon Verified Permissions.

## What is on the `Awesome` list

- Cedar official resources. Contents and repos from Amazon or CNCF are considered official. These are highlighted with :office:
- Community content that is still relevant or kept up-to-date by the author/community. 
- Community GitHub projects that are active and maintained with at least one release in last 6 months are included in this list.
  - Active: Projects with recent release within 3 months. These projects are highlighted with a :zap:
- Blogs, videos and research papers are sorted by latest on top.


## Contents

- [Official](#official)
- [Deploy and Run Cedar](#deploy-and-run-cedar)
- [Language and Platform Integrations](#language-and-platform-integrations)
  - [Official Bindings](#official-bindings)
  - [Community Bindings](#community-bindings)
  - [Framework and Platform Integrations](#framework-and-platform-integrations)
- [IDE and Editor Extensions](#ide-and-editor-extensions)
- [Tools](#tools)
- [Playgrounds and Policy Editors](#playgrounds-and-policy-editors)
- [Examples and Reference Applications](#examples-and-reference-applications)
- [Papers and Research](#papers-and-research)
- [Blogs and Articles](#blogs-and-articles)
- [Videos](#videos)
- [Contributing](#contributing)

## Official

- [Cedar Project](https://cedarpolicy.com/) - Project home, with an interactive playground, a ten-step tutorial and learning resources. :office:
- [Cedar Docs](https://docs.cedarpolicy.com/) - Language reference, syntax guide and best practices. :office:
- [Cedar Playground](https://cedarpolicy.com/en/playground) - Write policies and evaluate authorization requests in the browser, no install required. :office:
- [CNCF Project Page](https://www.cncf.io/projects/cedar/) - The page for Cedar as a CNCF Sandbox project, accepted in October 2025. :office:
- [Cedar on GitHub](https://github.com/cedar-policy) - The GitHub organization hosting the language, its proofs and its official integrations. :office:
- [cedar](https://github.com/cedar-policy/cedar) - The reference implementation of the Cedar language, in Rust. :office:
- [cedar-spec](https://github.com/cedar-policy/cedar-spec) - The Lean formalization of Cedar, plus the differential-testing harness that keeps the Rust implementation honest. :office:
- [cedar-examples](https://github.com/cedar-policy/cedar-examples) - Official sample applications, including TinyTodo, the app built by the docs tutorial. :office:
- [RFCs](https://github.com/cedar-policy/rfcs) - The design process for language changes, and the best place to see where Cedar is heading. :office:
- [Integration tests](https://github.com/cedar-policy/cedar-integration-tests) - Official integration tests for Cedar implementations. :office:
- [cedar-json-parser](https://github.com/cedar-policy/cedar-json-parser) - A JSON parser for Cedar, verified with Verus. :office:
- [Cedar Community](https://github.com/cedar-policy/cedar-community) - Notes from the monthly community meetings. :office:
- [Community Slack](https://cloud-native.slack.com/archives/C0AQXC9M4G1) - The Cedar channel on CNCF Slack. Get an invite at [slack.cncf.io](https://slack.cncf.io). :office:

## Deploy and Run Cedar

- [Amazon Verified Permissions](https://aws.amazon.com/verified-permissions/) - Managed AWS service for storing Cedar policies and evaluating authorization requests at scale. :office:
- [cedar-local-agent](https://github.com/cedar-policy/cedar-local-agent) - Official Rust crate for running a local decision point with file-backed policy and entity providers that reload on change. :office:
- [Cedarling](https://docs.jans.io/stable/cedarling/) - Open-source embeddable Cedar policy decision point with a Rust core. Offers 10 language [bindings](https://docs.jans.io/stable/cedarling/tutorials/cedarling-getting-started/), JWT token mapping and validation. Support policy store format to support policy governance and distribution. :zap:
- [Cedrus](https://github.com/stratusmedia/cedrus) - REST API server for Cedar Policy authorization, designed for internal infrastructure. It provides a multi-tenant authorization service.


## Language and Platform Integrations

### Official Bindings

- [cedar-java](https://github.com/cedar-policy/cedar-java) - Java bindings for the Cedar engine. :office:
- [cedar-go](https://github.com/cedar-policy/cedar-go) - Native Go implementation of Cedar, with no CGO or WASM required. :office:
- [cedar-authorization](https://github.com/cedar-policy/cedar-authorization) - TypeScript authorization primitives for building Cedar-backed enforcement points. :office:
- [cedar-wasm](https://www.npmjs.com/package/@cedar-policy/cedar-wasm) - WebAssembly build of the Cedar engine for JavaScript and browser use. :office:
- [highlightjs-cedar](https://github.com/cedar-policy/highlightjs-cedar) - Cedar syntax highlighting for highlight.js. :office:
- [prism-cedar](https://github.com/cedar-policy/prism-cedar) - Cedar syntax highlighting for Prism. :office:
- [cedar-monaco-editor](https://github.com/cedar-policy/cedar-monaco-editor) - Browser Cedar editor component wrapping Monaco, for building your own playground. :office:

### Community Bindings

- [cedar-py](https://github.com/k9securityio/cedar-py) - Python bindings for Cedar. :zap:
- [cedar-policy-rb](https://github.com/elct9620/cedar-policy-rb) - Ruby bindings for Cedar. :zap:
- [monocloud-cedar-dotnet](https://github.com/monocloud/monocloud-cedar-dotnet) - Alternative C#/.NET port, derived from the Java bindings.
- [tree-sitter-cedar](https://github.com/SwornSystems/tree-sitter-cedar) - Tree-sitter grammar for Cedar, used by editors for parsing and highlighting. :zap:
- [Cedarling-Rust](https://docs.jans.io/stable/cedarling/tutorials/rust/) - Run Cedar policy decision point in Rust application :zap:
- [Cedarling-WebAssembly](https://docs.jans.io/stable/cedarling/tutorials/javascript/) - Run Cedar policy decision point in browser. Embed into JavaScript based apps. Published to npm as `@janssenproject/cedarling_wasm`. :zap:
- [Cedarling-Python](https://docs.jans.io/stable/cedarling/tutorials/python/) - Run Cedar policy decision point in Python application. Published to PyPI as `cedarling-python`. :zap:
- [Cedarling-Java](https://docs.jans.io/stable/cedarling/tutorials/java/) - Run Cedar policy decision point in Java applications. :zap:
- [Cedarling-Go](https://docs.jans.io/stable/cedarling/tutorials/go/) - Run Cedar policy decision point in Go applications. :zap:
- [Cedarling-C](https://docs.jans.io/stable/cedarling/tutorials/c/) - C bindings, and the base for embedding in other native languages. :zap:
- [Cedarling-Kotlin](https://docs.jans.io/stable/cedarling/tutorials/kotlin/) - Run Cedar policy decision point in Kotlin applications. :zap:
- [Cedarling-Android](https://docs.jans.io/stable/cedarling/developer/mobile-apps/cedarling-android/) - Run Cedar policy decision point in Android application. :zap:
- [Cedarling-iOS](https://docs.jans.io/stable/cedarling/developer/mobile-apps/cedarling-ios/) - Run Cedar policy decision point in iOS application. :zap:
- [Cedarling-UniFFI](https://docs.jans.io/stable/cedarling/developer/mobile-apps/cedarling-uniffi/) - The UniFFI layer that generates the Kotlin, Android and iOS bindings. :zap:

### Framework and Platform Integrations

- [Cedar for Kubernetes](https://github.com/cedar-policy/cedar-access-control-for-k8s) - Authorize and admit Kubernetes API requests with Cedar policies. :office:
- [authorization-for-expressjs](https://github.com/cedar-policy/authorization-for-expressjs) - Official Express middleware that enforces Cedar policies on HTTP routes. :office:
- [cedar-for-agents](https://github.com/cedar-policy/cedar-for-agents) - Official exploration of Cedar for authorizing AI agents and their tool calls. :office:
- [Cedarling-sidecar](https://docs.jans.io/stable/cedarling/developer/sidecar/cedarling-sidecar-overview/) - Run Cedar policy decision point as a separate Flask container that support [AuthZEN API](https://openid.github.io/authzen/) :zap:

## IDE and Editor Extensions

- [VS Code](https://github.com/cedar-policy/vscode-cedar) - Official extension with syntax highlighting, validation and schema support ([Marketplace](https://marketplace.visualstudio.com/items?itemName=cedar-policy.vscode-cedar)). :office:

## Tools

- [cedar-policy-cli](https://docs.rs/cedar-policy-cli) - Official command-line tool to validate, format, translate and evaluate Cedar policies. :office:
- [Cedar Analysis (SymCC)](https://docs.rs/cedar-policy-symcc) - Symbolic compiler that translates policies to SMT, so you can prove equivalence, subsumption, disjointness and never-errors properties. The analysis itself is verified in Lean. :office:
- [cedar-policy-formatter](https://docs.rs/cedar-policy-formatter) - Official formatter library for Cedar policy source. :office:

## Playgrounds and Policy Editors

- [AgamaLab policy designer](https://cloud.gluu.org/agama-lab/dashboard/policy-designer)
- [OpenPARC Playground](https://playground.openparc.dev/)
- [cedarling.dev](https://cedarling.dev)

## Examples and Reference Applications

- [cedar-examples](https://github.com/cedar-policy/cedar-examples) - Official examples, including the TinyTodo tutorial application. :office:
- [AuthZEN interface for Verified Permissions](https://github.com/aws-samples/sample-authzen-interface-verified-permissions) - Reference implementation connecting the OpenID AuthZEN protocol to Amazon Verified Permissions. :office:
- [ASP.NET Core authorization provider](https://github.com/aws-samples/amazon-verified-permissions-asp-dotnet-core-custom-auth-policy-provider) - Custom ASP.NET Core authorization policy provider backed by Verified Permissions. :office:
- [RBAC to PBAC migration sample](https://github.com/aws-samples/sample-app-migrate-access-rbac-to-pbac-with-verified-permissions) - Worked example of migrating from role-based to policy-based authorization. :office:

## Papers and Research

- [SymCert: Verifying SMT-based policy analyses](https://www.amazon.science/publications/symcert-verifying-smt-based-policy-analyses) - Establishes the correctness of the SMT-based analyses that Cedar Analysis relies on.
- [How We Built Cedar: A Verification-Guided Approach](https://arxiv.org/abs/2407.01688) - How proofs, property-based testing and differential testing were used throughout development.
- [Cedar: A New Language for Expressive, Fast, Safe, and Analyzable Authorization](https://arxiv.org/abs/2403.04651) - The OOPSLA 2024 paper introducing the language and its design goals.

## Blogs and Articles

- [Policy Debate: Rego v CEL v Cedar](https://gluufederation.medium.com/policy-debate-rego-v-cel-v-cedar-24cc7a531bbc) - Comparing Cedar with Rego and CEL
- [Schema is Cedar's Superpower](https://medium.com/@gluufederation/schema-is-cedars-super-power-607920de55fb) - How schema helps in making Cedar policies more understandable and maintainable.
- [Composition - Formal Verification's Superpower](https://gluufederation.medium.com/composition-formal-verifications-superpower-1034f55ea9d3) 
- [When you need Cedar even if you love OPA](https://gluufederation.medium.com/when-you-need-cedar-even-if-you-love-opa-66a2ccd62b27)
- [Zanzibar Graphs Describe the World. Policies Govern It](https://gluufederation.medium.com/zanzibar-graphs-describe-the-world-policies-govern-it-e379615f61b5)
- [Mandate or Mission — Cedar v Markdown](https://gluufederation.medium.com/mandate-or-mission-cedar-v-markdown-e169ff509a04)
- [The Multi-Token AuthZ Challenge](https://gluufederation.medium.com/the-multi-token-authz-challenge-d8a2ef28cf49)
- [AWS Verified Permissions and Cedar Policy Language Complete Guide](https://hidekazu-konishi.com/entry/aws_verified_permissions_cedar_complete_guide.html) - A long-form reference covering the language and the managed service.
- [Cedar Joins CNCF as a Sandbox Project](https://aws.amazon.com/blogs/opensource/cedar-joins-cncf-as-a-sandbox-project/) - The donation announcement, and what it means for governance.
- [All About Cedar, an Open Source Solution for Fine-Tuning Kubernetes Authorization](https://thenewstack.io/all-about-cedar-an-open-source-solution-for-fine-tuning-kubernetes-authorization/) - Deep dive on the Kubernetes integration.
- [Migrating from Open Policy Agent to Amazon Verified Permissions](https://aws.amazon.com/blogs/security/migrating-from-open-policy-agent-to-amazon-verified-permissions/) - Practical guidance for moving Rego policies to Cedar.
- [Test Cedar in Your Browser](https://medium.com/janssen-project-feed/test-cedar-in-your-browser-2bd88c4e859f) - A nifty tool to test Cedar policies in your browser.
- [Introducing Cedar Analysis](https://aws.amazon.com/blogs/opensource/introducing-cedar-analysis-open-source-tools-for-verifying-authorization-policies/) - Launch post for the open source policy verification tooling.
- [Cedar Brings Fine-Grained Authorization to Kubernetes](https://www.infoq.com/news/2025/04/cedar-kubernetes-authorization/) - InfoQ coverage of the Kubernetes authorizer.
- [Cedar: A new approach to policy management for Kubernetes](https://www.cncf.io/blog/2025/03/28/cedar-a-new-approach-to-policy-management-for-kubernetes/) - CNCF blog on using Cedar for cluster authorization.
- [Paper review: Cedar, a new language for authorization](https://muratbuffalo.blogspot.com/2025/03/cedar-new-language-for-expressive-fast.html) - A readable walkthrough of the OOPSLA paper.
- [Simplifying Just-in-Time Access Governance using Cedar](https://www.commonfate.io/blog/jit-using-cedar) - Applying Cedar to time-bound access grants.
- [Two New Open Source Rust Crates Create Easier Cedar Policy Management](https://aws.amazon.com/blogs/opensource/easier-cedar-policy-management/) - Introduces the local agent and policy management crates.
- [How we designed Cedar to be intuitive to use, fast, and safe](https://aws.amazon.com/blogs/security/how-we-designed-cedar-to-be-intuitive-to-use-fast-and-safe/) - The language design tradeoffs behind the syntax and evaluation model.
- [Implementing Role-Based Access Control (RBAC) with Cedar](https://www.permit.io/blog/cedar-rbac) - Modelling roles and permissions in Cedar.
- [The Cedar Programming Language: Authorization Simplified](https://thenewstack.io/the-cedar-programming-language-authorization-simplified/) - An accessible overview of what Cedar is for.
- [Scaling Authorization with Cedar and OPAL](https://www.permit.io/blog/scaling-authorization-with-cedar-and-opal) - Distributing Cedar policy and data updates in real time.
- [Cedar vs Rego (OPA)](https://www.permit.io/blog/opa-vs-cedar) - Compares Cedar and Rego on syntax, analyzability and tooling.
- [How we built Cedar with automated reasoning and differential testing](https://www.amazon.science/blog/how-we-built-cedar-with-automated-reasoning-and-differential-testing) - The verification story, written for a general audience.
- [Using Open Source Cedar to Write and Enforce Custom Authorization Policies](https://aws.amazon.com/blogs/opensource/using-open-source-cedar-to-write-and-enforce-custom-authorization-policies/) - A hands-on introduction to embedding Cedar in an application.
- [Technometria Blog](https://www.technometria.com/) - 
    - [Delegation as Data: Applying Cedar Policies to OpenClaw Subagents](https://www.technometria.com/p/delegation-as-data-applying-cedar)
    - [A Policy-Aware Agent Loop with Cedar and OpenClaw](https://www.technometria.com/p/a-policy-aware-agent-loop-with-cedar)
    - [Childproofing the Control Plane: Using Cedar to Build Frontal Lobes for Agentic Systems](https://www.technometria.com/p/childproofing-the-control-plane-using)
    - [Beyond Denial: Using Policy Constraints to Guide OpenClaw Planning](https://www.technometria.com/p/beyond-denial-using-policy-constraints)
    - [Human in the Loop Control for OpenClaw](https://www.technometria.com/p/human-in-the-loop-control-for-openclaw)
    - [Authorization Before Retrieval: Making RAG Safe by Construction](https://www.technometria.com/p/authorization-before-retrieval-making)
    - [Zero Trust, Least Privilege, and Just-in-Time Access](https://www.technometria.com/p/zero-trust-least-privilege-and-just)
  - [A Gentle Introduction to Automated Reasoning](https://www.amazon.science/blog/a-gentle-introduction-to-automated-reasoning)
  - [White paper introducing Cedar](https://arxiv.org/pdf/2403.04651)

## Videos 

- [AWS re:Invent 2022 - Use policies to manage permissions](https://www.youtube.com/watch?v=k6pPcnLuOXY) - The session that introduced Verified Permissions and Cedar.
- [How MongoDB uses Cedar policy language for fine-grained authorization](https://www.youtube.com/watch?v=Ui7cFy23Y9o)
- [Hooking Coding Agents with the Cedar Policy Language](https://www.youtube.com/watch?v=m6pzrqFJ6hE) - Matt Maisel on using Cedar to constrain AI coding agents.
- [Top 5 reasons to use Cedar](https://www.youtube.com/live/b4gxRzadung) - Discussion with Emina Torlak
- [Cedar analysis toolkit](https://www.youtube.com/live/wtdbLLUKXTw) - Discussion with Spencer Erickson and Liana Hadarean
- [Amazon's Cedar Open Source Strategy with Ricardo Sueiras and Julian Lovelock](https://www.youtube.com/live/FIIiAcRUe5o) - Discussion with Ricardo Sueiras and Julian Lovelock
- [Agentic Authorization with Cedar Sarah Cecchetti](https://www.youtube.com/live/zjFPsZenLtk)
- [CNCF Cedar Update John Kastner](https://www.youtube.com/live/AjjI88INORc)
- [How Cedar Simplies Authz for Developers](https://www.youtube.com/watch?v=ptNWUn8DVZQ) - Discussion with Dinesh Rajasekharan
- [Dynamic Authorization Update with Phil Windley](https://www.youtube.com/live/AxwzCZsc3nI)
- [Cedar Gets Temporal: Meet Dogwood (with Marc Brooker)](https://www.youtube.com/live/v98lD7YmYnk)
- [Discover Cedar: AWS New Open-Source Policy Language](https://www.youtube.com/watch?v=E4-mCWSsQFc) - An introductory walkthrough of the language.
- [Enforcing Consent Conformance in Your Authz Logic with a Fine-Grained Perms Model (Identiverse 2023)](https://www.youtube.com/watch?v=HnnlGBNur2w) - Consent modelling with a fine-grained permissions model, featuring Cedar.
- [AWS On Air - featuring Open Source Security at AWS](https://www.youtube.com/watch?v=T8X7VDmJkz4) - Includes a discussion of Cedar and a demo.
- [Demo of the Cedar Programming Language](https://www.youtube.com/watch?v=PzmDYyyA5xM) - A short live demo of writing and evaluating policies.
- [Use policies to manage permissions with Amazon Verified Permissions (re:Invent 2022)](https://www.youtube.com/watch?v=k6pPcnLuOXY) - The session that introduced Verified Permissions and Cedar.

## Books

- [Authorization in Action](https://www.manning.com/books/authorization-in-action) - by Phil Windley - The book uses Cedar to explain the concepts of authorization and also as a practical implementation. Great book to get started with authorization in general.

## Contributing

Built an awesome Cedar integration or wrote an interesting blog or article on the topic? Submit a Pull Request! Just follow the [guidelines](https://github.com/cedar-policy/.github/blob/main/CONTRIBUTING.md).
