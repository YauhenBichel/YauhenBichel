# Yauhen Bichel

### Staff Software Engineer · AI platforms, distributed backends, self-hosted LLM systems
**London, United Kingdom**

> **Open to Staff / Principal / Lead engineering roles — AI & ML platforms,
> data infrastructure and distributed backends. London or remote.**
> [yauhen.bichel@gmail.com](mailto:yauhen.bichel@gmail.com) ·
> [LinkedIn](https://www.linkedin.com/in/yauhen-bichel) ·
> [Medium](https://medium.com/@yauhen.bichel) ·
> [Hugging Face](https://huggingface.co/YauhenBichel)

## What I do

I build the systems around AI models rather than the models themselves: the gateways
that route requests, the runtimes that run agents, the evaluation harnesses that say
whether an agent is any good, and the infrastructure that keeps all of it up. Fourteen
years of backend work came first — Kafka event pipelines, Spark batch jobs, Spring and
Python services, Terraform for AWS and Azure — and that is still where most of my
judgement comes from.

Today I am a **Staff Software Engineer and one of the main maintainers of
[OpenSRE](https://github.com/tracer-Cloud/opensre)** (Apache-2.0 framework for AI SRE
agents, 11k+ ★), where I own the agent runtime and the evaluation platform. I co-founded
[MoleCare](https://molecare.co.uk), a skin-lesion monitoring app accepted onto the NHS
Apps Library, and still run it.

**Python · Java · Go · TypeScript · C#/.NET** on **AWS · GCP · Azure** · Terraform certified

---

## yserver: my local LLM system

One small AMD computer with 128 GB of shared memory serves open models to Claude Code,
my editor and my scripts. A gateway speaking the OpenAI and Anthropic APIs routes each
request to a role-specific model — coding, reasoning, judge, vision, OCR, speech — behind
a queue, with tracing on every hop. Everything below runs on it or was built for it.

**[yserver-local-llm-system](https://github.com/YauhenBichel/yserver-local-llm-system)** — the system described in full:
the architecture, [ten flows with diagrams](https://github.com/YauhenBichel/yserver-local-llm-system/blob/main/docs/flows.md),
[the measured numbers](https://github.com/YauhenBichel/yserver-local-llm-system/blob/main/docs/numbers.md)
(0.64 s to the first token, 50 tokens per second, 132 requests with 0 failures), and
[seven lessons](https://github.com/YauhenBichel/yserver-local-llm-system/blob/main/docs/lessons.md),
most of which are not about models.

*Operating it*

- **[llm-hops](https://github.com/YauhenBichel/llm-hops)** — see every hop of a request through a local LLM system: a tracing server, a live flow map and a waterfall per request. One static binary. Built after the 40-second answer whose time went nowhere I could see.
- **[silent-failures](https://github.com/YauhenBichel/silent-failures)** — small read-only checks for the failures that stay silent: a hardware watchdog that never loads, a nightly job that fails every night, firmware months behind upstream, a box that froze and nobody was told.
- **[homerunner](https://github.com/YauhenBichel/homerunner)** — run your private repositories' CI on a machine you already own. One command per repo, and it refuses to register against a public repo, where anyone's pull request would run code on your machine.
- **[strix-halo-jax](https://github.com/YauhenBichel/strix-halo-jax)** — JAX and MuJoCo MJX on an AMD Ryzen AI MAX iGPU from pip wheels, no system ROCm, with a hang-safe check that tells you which wheel set works.

*Choosing and using models*

- **[moe-fit](https://github.com/YauhenBichel/moe-fit)** — will this mixture-of-experts model run on my machine, and how fast? Answered from the model's index before the download. [![PyPI](https://img.shields.io/pypi/v/moe-fit.svg)](https://pypi.org/project/moe-fit/)
- **[py-harness](https://github.com/YauhenBichel/py-harness)** — a local 8B model behind a typed one-action-per-turn harness: ask a question, write a test, fix a bug, add one small function. Write jail, AST-validated patches, and it only touches the folder you point it at. [![PyPI](https://img.shields.io/pypi/v/py-harness-cli.svg)](https://pypi.org/project/py-harness-cli/)

*Speech and language, served the same way*

- **[belarusian-tts](https://github.com/YauhenBichel/belarusian-tts)** — natural, self-hostable Belarusian text-to-speech behind an OpenAI-style `/v1/audio/speech`.
- **[belarusian-asr](https://github.com/YauhenBichel/belarusian-asr)** — Belarusian speech recognition on the CPU: an OpenAI- and whisper.cpp-compatible server with a FLEURS benchmark.
- **[belarusian-verse](https://github.com/YauhenBichel/belarusian-verse)** — stress, rhyme, rhythm and agreement checking for Belarusian, built on the Grammar Database. The songs it helps write are on [TikTok](https://www.tiktok.com/@y6574694).

*Things with a face*

- **[humanoid-companion](https://github.com/YauhenBichel/humanoid-companion)** — a small humanoid robot that walks with a reinforcement-learned policy, shows a face with lip sync and speaks; its brain is the local LLM. MuJoCo simulation, sim-to-real.
- **[humanoid-desktop](https://github.com/YauhenBichel/humanoid-desktop)** — the same teammate floating on a Mac desktop, in Swift.

## Writing

On [Medium](https://medium.com/@yauhen.bichel), mostly about running this system and what it taught me:

- [I sent a prompt that was too long. The server answered someone else's question.](https://medium.com/@yauhen.bichel/i-sent-a-prompt-that-was-too-long-the-server-answered-someone-elses-question-3757a17c52a7) — September 2026
- [Ten days with my home server: how I made it fast, stable and able to work alone](https://medium.com/@yauhen.bichel/ten-days-with-my-home-server-how-i-made-it-fast-stable-and-able-to-work-alone-dab7a26f290e) — September 2026
- [I built my own LLM system at home](https://medium.com/@yauhen.bichel/i-built-my-own-llm-system-at-home-e92514a3b2be) — September 2026
- [I tried a small open LLM for daily Python. Here is what I got.](https://medium.com/@yauhen.bichel/i-tried-a-small-open-llm-for-daily-python-here-is-what-i-got-a7c122f06a05) — August 2026
- [I am building a cheap LLM for everyday Python vibe coding](https://medium.com/@yauhen.bichel/i-am-building-a-cheap-llm-for-everyday-python-vibe-coding-come-join-3aaa32f72d2a) — August 2026
- [Terraform provisioning and CI/CD with GitHub Actions: my design and implementation](https://medium.com/@yauhen.bichel/my-design-and-implementation-of-terraform-provisioning-and-cicd-with-github-actions-workflow-for-ba0469743531) — August 2025
- [Know your resources in an AWS account and feel calm about changes](https://medium.com/@yauhen.bichel/know-your-resources-in-aws-account-and-feel-calm-with-changes-in-your-aws-account-1b77c521ace2) — July 2025
- [Risks in AI development: Google's SAIF risk map](https://medium.com/@yauhen.bichel/risks-in-ai-development-google-saif-risk-map-1d59d2d3dfa8) — November 2024

---

## Open source I maintain

**[molecare-mcp](https://github.com/MoleCare/molecare-mcp)** — MCP server giving Claude
and other clients educational dermatology knowledge: lesion terminology, ABCDE criteria,
SNOMED CT to ICD-10 mapping. Runs with no credentials.
[![npm](https://img.shields.io/npm/v/molecare-mcp)](https://www.npmjs.com/package/molecare-mcp)
[![downloads](https://img.shields.io/npm/dw/molecare-mcp)](https://www.npmjs.com/package/molecare-mcp)

```bash
npx -y molecare-mcp
```

**[molecare-ml](https://github.com/MoleCare/molecare-ml)** — the melanoma classifier behind
MoleCare, published with a model card that states plainly what was *not* measured. Its
[write-up on why 94% accuracy means very little](https://github.com/MoleCare/molecare-ml/blob/main/doc/94-percent-accurate.md)
explains the gap, and the open
[bias evaluation issue](https://github.com/MoleCare/molecare-ml/issues/10) is the problem
I would most like help with: performance across Fitzpatrick skin types is unmeasured, and
dermoscopic datasets under-represent darker skin.

**[molecare-desktop](https://github.com/MoleCare/molecare-desktop)** · **[molecare-skin-llm](https://github.com/MoleCare/molecare-skin-llm)** — the Electron desktop build, and a LoRA-tuned educational Q&A model behind a deterministic safety harness.

None of it is a medical device. None of it diagnoses anything.

## Tools I publish

**[merge-cheer](https://github.com/YauhenBichel/merge-cheer)** — a GitHub Action
that comments a G-rated GIF when a pull request merges. No Giphy key, no secrets,
and it ships its own loops so it works on a new repository with the default token.

**[readme-contributors](https://github.com/YauhenBichel/readme-contributors)** — a
GitHub Action that draws the contributors wall further down this page. Circular
avatars, no table, bots omitted.

**[regex-parity](https://github.com/YauhenBichel/regex-parity)** — the same regex gives
different answers in JavaScript, Python and Java on real-world text. This makes the rules
agree across languages, and proves it. [Live demo](https://yauhenbichel.github.io/regex-parity/).

## Also built

**Infrastructure and tooling**

- **[terraform-aws-parameter-store](https://github.com/YauhenBichel/terraform-aws-parameter-store)** — Terraform module for AWS Parameter Store.
- **[terraform-aws-eventbridge-batch-trigger](https://github.com/YauhenBichel/terraform-aws-eventbridge-batch-trigger)** — Terraform module for EventBridge-triggered AWS Batch jobs.
- **[terraform-aws-batch-job-revision](https://github.com/YauhenBichel/terraform-aws-batch-job-revision)** — Terraform module for AWS Batch job revisions.
- **[github-action-terraform-output](https://github.com/YauhenBichel/github-action-terraform-output)** — GitHub Action that reads Terraform output.
- **[tracer-sre-rl](https://github.com/YauhenBichel/tracer-sre-rl)** — reinforcement learning for AI SRE agents: training LLM-based agents to diagnose and remediate production incidents.

**Services and applications**

- **[demo-openlr-mapbox-data](https://github.com/YauhenBichel/demo-openlr-mapbox-data)** — Decoding OpenLR location references against Mapbox data.
- **[Services-with-Mesh-and-gRPC](https://github.com/YauhenBichel/Services-with-Mesh-and-gRPC)** — Microservices over gRPC behind a service mesh.
- **[Text-to-image-RESTful-service](https://github.com/YauhenBichel/Text-to-image-RESTful-service)** — REST API for Stable Diffusion image generation.
- **[Retry-with-resilience4j](https://github.com/YauhenBichel/Retry-with-resilience4j)** — Retry policies with resilience4j.
- **[AudioPlayer](https://github.com/YauhenBichel/AudioPlayer)** — React Native audio player for iOS.

## Contributions

Over 1,000 merged pull requests across roughly 97 repositories, mostly on the projects
above and in the [MoleCare](https://github.com/MoleCare) organisation, plus 330 merged
pull requests on [OpenSRE](https://github.com/Tracer-Cloud/opensre), where I am one of
the main maintainers.

---

## Contributors

Thank you to everyone who has helped.

<!-- readme: contributors,bots/- -start -->
<p align="center">
  <a href="https://github.com/YauhenBichel" title="Yauhen Bichel" aria-label="Yauhen Bichel"><img src=".github/faces/YauhenBichel.svg" width="87" height="99" alt="Yauhen Bichel" /></a>
</p>
<!-- readme: contributors,bots/- -end -->

Filled from GitHub commits (bots omitted). Live demo: [readme-contributors](https://github.com/YauhenBichel/readme-contributors#live-demo).
