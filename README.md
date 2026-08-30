# Yauhen Bichel

### Software Engineer / Platform Engineer / ML Engineer and AI agentic contributor
**London, United Kingdom**

> **Open to Staff / Principal / Lead engineering roles — AI & ML platforms,
> data infrastructure and distributed backends. London or remote.**
> [yauhen.bichel@gmail.com](mailto:yauhen.bichel@gmail.com) ·
> [LinkedIn](https://www.linkedin.com/in/yauhen-bichel) ·
> [Medium](https://medium.com/@yauhen.bichel)

Software engineer with **14+ years** building agentic AI applications, ML systems,
big data pipelines, distributed backends and cloud infrastructure. I build systems
from scratch — from CNN training and TensorFlow serving, through Kafka event
pipelines and Spark/HDFS batch computation, to the Terraform that provisions all of it.

**Java · Go · Python · Node.js · C#/.NET** on **AWS · GCP · Azure**

Currently a core open-source contributor to [OpenSRE](https://github.com/tracer-Cloud/opensre)
(Apache-2.0 framework for AI SRE agents, 10k+ ★) and co-founder of
[MoleCare](https://molecare.co.uk), a skin-lesion monitoring app published on the
NHS App Library.

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

**[molecare-webapp](https://github.com/MoleCare/molecare-webapp)** · **[molecare-desktop](https://github.com/MoleCare/molecare-desktop)** · **[skincare-qa](https://github.com/MoleCare/skincare-qa)** — the React front end, the Electron desktop build, and a LoRA-tuned educational Q&A model.

None of it is a medical device. None of it diagnoses anything.

---
