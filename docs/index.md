# EVE: Earth Virtual Expert

<table>
<tr>
<td width="32%" align="center" valign="middle">

<img src="./assets/EVE_SCIENTIST_AVATAR_.png" width="210" alt="EVE Avatar">

</td>
<td width="68%" align="left" valign="middle">

<b>Earth Virtual Expert (EVE)</b>  
An open science initiative funded and supported by the <b>European Space Agency's Φ-lab</b>, developed by <b>Pi School</b> in collaboration with <b>Imperative Space</b> and <b>Mistral AI</b>, aimed at advancing the use of <b>Large Language Models (LLMs)</b> for the Earth Observation (EO) and Earth Science (ES) communities.

</td>
</tr>
</table>

## Use EVE

EVE is open to everyone at [eve-chat.chat](https://eve-chat.chat). Sign up with the EVE identity provider and confirm your email address with the code it sends you. Sign-in, password reset, and optional two-factor authentication also happen at the identity provider.

- [Chat](frontend/docs/features/chat.md): ask questions and get answers with sources.
- [Control panel](frontend/docs/features/control_panel.md): tune retrieval and generation parameters.
- [Private collections](frontend/docs/features/private_collection.md): upload your own documents and search them.
- [Profile](frontend/docs/features/profile.md): manage your account details.

## Build with EVE

EVE exposes an OpenAI-compatible API at `https://eve-chat.chat/api/v1`. Authenticate with an API key that you create in the chat platform.

- [API keys in the chat platform](frontend/docs/features/api-keys.md): create, copy, and revoke a key.
- [API keys reference](backend/docs/api/api-keys.md): the key management endpoints.
- [OpenAI-compatible gateway](backend/docs/api/openai-gateway.md): models, token budget, and an SDK example.
- [Swagger API](backend-swagger.md): the full backend API reference.

## Components

This guide documents the components that power EVE. They are open source and designed to be reused in research on LLMs for Earth Observation.

- **[Chat frontend](frontend/docs/index.md)**: the web application of the EVE chat platform.
- **[Chat backend](backend/docs/index.md)**: the API behind the chat platform.
- **[Evalkit](evalkit/docs/index.md)**: an evaluation framework for LLMs on EO tasks and general domain benchmarks.
- **[Data scraping](data-scraping/docs/index.md)**: a framework to collect EO documents from trusted sources.
- **[Data processing](data-processing/docs/index.md)**: a pipeline to clean, filter, chunk, and embed EO documents.

The project also publishes experiment repositories with hands-on notebooks. They are not production code and are not part of this guide:

- **[EVE-RAG](https://github.com/eve-esa/eve-rag)**: build and benchmark Retrieval-Augmented Generation (RAG) systems.
- **[EVE-Hallucination](https://github.com/eve-esa/eve-hallucination)**: experiments and analysis on the hallucination pipeline of EVE.

## Project overview

EVE is a domain-specialized AI system that supports **scientists, analysts, and decision-makers** through natural-language interaction.

It assists with tasks such as:

- EO and ES knowledge search and summarisation
- Scientific Q&A and policy brief generation
- Document understanding and retrieval
- Technical and educational content creation
- Search across private EO document collections through RAG

The project unites **data curation, model development, evaluation, and deployment** to deliver open, reusable tools for Europe's EO ecosystem.

## Model

`EVE-Instruct` is trained on domain-curated corpora by fine-tuning **Mistral Small 3.2 24B**, through **continued pretraining** and **instruction fine-tuning**.

- The model is optimized for factuality, reasoning, and integration with retrieval-augmented generation.
- Training was carried out using **EuroHPC MareNostrum**, cloud environments, and **Mistral infrastructure**.
- Evaluation targets both **general domain** and **EO-specific** benchmarks.

In the chat platform, EVE-Instruct is the default model. The **Jülich Supercomputing Centre (JSC)** serves it through its Blablador inference service, and backup providers answer when JSC is unavailable.

## Licence

All EVE releases follow **ESA and EU open-science principles**, promoting transparency, reproducibility, and European AI sovereignty.  
The project's outputs (**models, datasets, pipelines, and documentation**) are shared under **permissive open-source licences** (Apache 2.0 or CC-BY).

## Links

- **Chat platform**: [eve-chat.chat](https://eve-chat.chat)
- **Project website**: [eve.philab.esa.int](https://eve.philab.esa.int/), project updates and communication materials.
- **Models and data**: [huggingface.co/eve-esa](https://huggingface.co/eve-esa), model checkpoints, datasets, and evaluation benchmarks.
- **Code**: [github.com/eve-esa](https://github.com/eve-esa), open-source tools, pipelines, and scripts.

## Contributors

- [European Space Agency (Φ-lab)](https://philab.esa.int/)
- [Pi School](https://picampus-school.com/)
- [Imperative Space](https://www.imperative.space/)
- [Mistral AI](https://mistral.ai/)
