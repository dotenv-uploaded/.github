<p align="center">
  <a href="https://github.com/dotenv-uploaded/_FOLDING_">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dotenv-uploaded/_FOLDING_/main/docs/assets/folding-logo-white.png">
      <img src="https://raw.githubusercontent.com/dotenv-uploaded/_FOLDING_/main/docs/assets/folding-logo.png" width="290" alt="Folding">
    </picture>
  </a>
</p>

<p align="center">
  Reads your documents, connects them,<br />
  and changes nothing without your approval.
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

<p align="center">
  <img src="./assets/folding-graph.png" width="100%" alt="Folding's knowledge graph: 119 documents and 285 relationships, colored by connected network" />
</p>

<p align="center"><sub>119 documents, 285 relationships. The colors are networks, not decoration.</sub></p>

### Relationships you can open and check

Converted HWP, DOCX and PDF files hold no links to one another, so counting explicit links would leave a
graph of isolated dots. Folding derives relationships from **entities that several documents share**, and
stores the sentence in which *each* side mentions them — expand a relationship and you read both, because
entity overlap has no direction. Entities appearing in nearly every document are thrown away: they connect
everything and distinguish nothing. Networks are named after the folder holding most of their members,
never by hand, so a network dominated by personal names announces itself.

### No API key. Nothing uploaded.

Conversion, analysis, retrieval and editing run on the machine in front of you, against a local model.
Signing in establishes **who you are**. Choosing a folder establishes **what Folding may read**. Neither
one implies the other.

### The agent asks before it acts

Rather than confining the agent to a short list of safe tools, every call passes an approval gate showing
the intended action, its risk, and **the request you actually made**. Prompt injection cannot be detected
perfectly, but an unexpected `rm` is obvious sitting next to "summarize this folder." No answer counts
as no.

### Edits that cannot quietly corrupt a file

A generic text editor destroys HWP and DOCX layout, so every format gets its own writer. Each one leaves
the source file untouched, reopens what it saved to confirm the change is really there, and never leaves
partial output that looks finished. PDF gets an annotated copy — Folding does not pretend PDF body text is
safely editable.

<p align="center">
  <a href="https://github.com/ghdtjdwn">@ghdtjdwn</a> ·
  <a href="https://github.com/Mingoomato">@Mingoomato</a> ·
  <a href="https://github.com/thddydgnl">@thddydgnl</a> ·
  <a href="https://github.com/Woochang4862">@Woochang4862</a>
</p>
