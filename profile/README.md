<p align="center">
  <a href="https://github.com/dotenv-uploaded/_FOLDING_">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dotenv-uploaded/_FOLDING_/main/docs/assets/folding-logo-white.png">
      <img src="https://raw.githubusercontent.com/dotenv-uploaded/_FOLDING_/main/docs/assets/folding-logo.png" width="300" alt="Folding">
    </picture>
  </a>
</p>

<p align="center">
  A local-first document agent that reads your files, connects them,<br />
  and edits them only with your approval.
</p>

<p align="center">
  <a href="https://github.com/dotenv-uploaded/_FOLDING_"><strong>Source code »</strong></a>
</p>

<p align="center">
  <a href="https://github.com/dotenv-uploaded/_FOLDING_#knowledge-graph">Knowledge graph</a> ·
  <a href="https://github.com/dotenv-uploaded/_FOLDING_#editing-documents">Document writers</a> ·
  <a href="https://github.com/dotenv-uploaded/_FOLDING_#approval-gate">Approval gate</a> ·
  <a href="https://github.com/dotenv-uploaded/_FOLDING_#architecture">Architecture</a> ·
  <a href="https://github.com/dotenv-uploaded/_FOLDING_/actions/workflows/desktop-installers.yml">Installers</a>
</p>

---

Conversion, analysis, retrieval and editing all run on the user's own computer, and no third-party AI API
key is required. Signing in establishes **who you are**. Choosing a folder establishes **what Folding may
read**. Signing in never grants access to local files.

<p align="center">
  <img src="./assets/folding-graph.png" width="100%" alt="Folding's knowledge graph: 119 documents and 285 relationships, colored by connected network" />
</p>

<p align="center"><em>The real interface — 119 documents, 285 relationships, colored by network.</em></p>

Converted HWP, DOCX and PDF files hold no links to one another, so counting explicit links would leave a
graph of isolated dots. Folding instead derives relationships from **entities that several documents
share**, and keeps the sentence in which *each* side mentions them. The result is a relationship you can
open and check, not a similarity score you have to take on faith.

- **Local by default.** The current local build answers with a model running on the user's machine through
  Ollama or LM Studio. Private documents do not need to leave the device to be useful.
- **Every tool call passes an approval gate.** The agent is not limited to a short safe-tool list; instead
  the interface shows what it intends to do, the risk, and *the user's original request*. No answer means
  denied.
- **Writers that respect the format.** Editing HWP or DOCX with a generic text editor destroys layout, so
  each format gets its own writer — one that never overwrites the source, reopens the saved file to confirm
  the change landed, and never leaves partial output behind.
- **PDF is treated honestly.** Folding does not pretend PDF body text is safely editable. It produces an
  annotated copy instead.

Built at the 2026 Codegate AI START UP Hackathon by team **.env 올려버린 팀** —
[@ghdtjdwn](https://github.com/ghdtjdwn) ·
[@Mingoomato](https://github.com/Mingoomato) ·
[@thddydgnl](https://github.com/thddydgnl) ·
[@Woochang4862](https://github.com/Woochang4862)
