# EVE — Earth Virtual Expert

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

## Getting started

In this documentation, you will find all the necessary information to understand, use, and contribute to the EVE project. The EVE project encompasses several components that have been open-sourced for the benefit of the EO community.
In this guide we provide the documentation for the components we built and used as part of the EVE project:

- **[Evalkit](./evalkit/docs)**: A comprehensive evaluation framework for assessing LLMs on EO-specific tasks and General Domain benchmarks.
- **[Data Scraping](./data-scraping/docs)**: Framework used to scrape relevant EO documents from trusted sources.
- **[Data Processing](./data-processing/docs)**: Comprehensive pipeline for cleaning, filtering, chunking and embedding EO documents.
- **[Chat-Backend](./backend/docs)**: Codebase that powers the backend of the EVE chat platform.
- **[Chat-Frontend](./frontend/docs)**: Codebase that powers the frontend of the EVE chat platform.

All these components represent the building blocks of the EVE project and are designed to be reusable and extensible for future research and development in the field of LLMs for Earth Observation.
You can navigate through the different sections of this documentation using the sidebar on the left. Each section provides detailed information, examples, and instructions to help you get started with EVE.

Other than these components, the EVE project also includes several repositories of experiments containing hands-on notebooks that have been included in the components above.
These experiments repositories are not part of the main documentation since they do not contain production-ready code, however they are a useful entry point for those who want a hands-on experience exploring the EVE project.
Here below the list of experiments repositories:

- **[EVE-RAG](https://github.com/eve-esa/eve-rag)**: A collection of notebooks demonstrating how to build Retrieval-Augmented Generation (RAG) systems and how to benchmark it.
- **[EVE-Hallucination](https://github.com/eve-esa/eve-hallucination)**: repository containing experiments and analysis on the hallucination pipeline implemented in EVE

## Project Overview

EVE is a domain-specialized AI system designed to support **scientists, analysts, and decision-makers** through natural-language interaction.

It provides expert assistance across tasks such as:

- EO and ES knowledge search and summarisation
- Scientific Q&A and policy brief generation
- Document understanding and retrieval
- Technical and educational content creation
- Integration of private EO document collections via RAG

The project unites **data curation, model development, evaluation, and deployment** to deliver open, reusable tools for Europe’s EO ecosystem.

## Chat Platform

EVE features an interactive **chat platform** that allows users to explore and query Earth Observation and Earth Science knowledge through natural dialogue.  
The platform is currently under **closed access** — you can request an early access to the beta version via this registration link [**here**](https://eve.philab.esa.int/pilot).  
It is targeted for **public release in early 2026**.

## Model Development

`EVE-Instruct` is trained on domain-curated corpora by fine-tuning **Mistral Small 3.2 24B**, through **continued pretraining** and **instruction fine-tuning**.

- The model is optimized for factuality, reasoning, and integration with retrieval-augmented generation.
- Training was carried out using **EuroHPC Marenostrum**, cloud environments, and **Mistral infrastructure**.
- Evaluation targets both **general domain** and **EO-specific** benchmarks.

## Licence

All EVE releases follow **ESA and EU open-science principles**, promoting transparency, reproducibility, and European AI sovereignty.  
The project’s outputs—**models, datasets, pipelines, and documentation**—are shared under **permissive open-source licences** (Apache 2.0 / CC-BY).

## Main Links

- 🌐 **Project Website** — [eve.philab.esa.int](https://eve.philab.esa.int/)  
  Central hub for project updates, communication materials, and registration for early access to the EVE chat platform.

- 🤗 **Models & Data** — [huggingface.co/eve-esa](https://huggingface.co/eve-esa)  
  Repository for domain-specific model checkpoints, datasets, and evaluation benchmarks.

- 💻 **Codebase** — [github.com/eve-esa](https://github.com/eve-esa)  
  Open-source tools, pipelines, and scripts developed within the EVE initiative.

## Contributors

<p align="center">
  <a href="https://philab.esa.int/" target="_blank">European Space Agency (Φ-lab)</a>
  <a href="https://picampus-school.com/" target="_blank">Pi School</a> ·
  <a href="https://www.imperative.space/" target="_blank">Imperative Space</a> ·
  <a href="https://mistral.ai/" target="_blank">Mistral AI</a> ·
</p>
