## Before you're done

This repo has been created for your AI Tour 2027 session. Here's how to get it ready.

**Easiest path — use the agent (recommended):**

- Open GitHub Copilot Chat and say `help me initialize repo`. The agent will walk you through getting the README populated.
- When you're ready to publish, say `help me finalize repo`. The agent will clean up unused folders, validate everything, and remove this "Before you're done" section and other extra stuff that attendees don't need to see.
- Curious how it works? Read the [agent workflow](.github/AGENT-WORKFLOW.md).

**Doing it manually?**

Fill in the sections below yourself, then:

- Delete any placeholder folders you don't need (`data/`, `infra/`, etc.)
- Delete this "Before you're done" section
- Delete `.github/agents/`, `.github/tests/`, `.github/copilot-instructions.md`, and `.github/AGENT-WORKFLOW.md` — these are template tooling, not part of your published repo

**Folder conventions:**

- Attendee step-by-step guidance goes in `instructions/`. If you use MkDocs or a docs site instead, put it in `docs/` and link to it from this README.
- Reference material and background reading go in `docs/`.
- Presenter notes, deck link, recordings, and re-delivery materials go in `delivery-resources/`. Fill in [`delivery-resources/README.md`](delivery-resources/README.md).
- You can add a `.devcontainer/` folder if needed.

---

<a name="start-building"></a>

<p align="center">
<img src="img/banner-ai-tour-27.png" alt="Microsoft AI Tour 2027" width="100%"/>
</p>

# [Microsoft AI Tour 2027](https://aitour.microsoft.com)

## 🔥 BRK231: Trusted AI at scale: Foundry to Agent 365

### Session description

Learn how Microsoft Foundry, GitHub Copilot, Copilot Studio, and Agent 365 work together to help organizations build, operationalize, govern, and scale AI agents across the enterprise with security, control, and trust.

> **Storyline:** The session follows **Caldova Pharmaceuticals**, a fictional global pharmaceutical company facing a sudden manufacturing capacity gap. Caldova's teams build a **supplier intelligence agent** in Copilot Studio, optimize an **invoice assurance agent** in Microsoft Foundry, and then **observe, onboard, and govern** every agent across the enterprise with Agent 365.

### 🚀 Getting started

#### In a guided session

If you're following along during a live session:

1. Watch the three demos: Copilot Studio, Microsoft Foundry, and Agent 365.
2. Scan the QR code on the closing slide, or visit [aka.ms/aitour27/BRK231](https://aka.ms/aitour27/BRK231), to open this repository.
3. After the session, open [`instructions/`](instructions/README.md) to try each step at your own pace.

#### On your own

If you're learning at your own pace:

1. Clone this repository.
2. Read [`docs/`](docs/README.md) for the Caldova scenario and the build, ground, secure and govern, and scale model.
3. Follow [`instructions/`](instructions/README.md) to explore Copilot Studio, Microsoft Foundry, and Agent 365.

### 🎯 Learning outcomes

By the end of this session, you will be able to:

- Explain how Microsoft Foundry, GitHub Copilot, Copilot Studio, and Agent 365 fit together across the enterprise AI agent lifecycle.
- Build and operationalize AI agents using Microsoft Foundry, GitHub Copilot, and Copilot Studio.
- Govern and scale AI agents with security, control, and trust using Agent 365.

### 🧩 The Caldova story in this session

| Act | What happens | Persona | Product |
|---|---|---|---|
| 1 | Understand the AI scale challenge: why pilots stall, and one connected system to build, ground, secure and govern, and scale agents | — | — |
| 2 | Build a conversational agent grounded in supplier contracts that recommends the best-fit contract manufacturer, with evidence | Charlotte Waltson, VP of Procurement | Microsoft Copilot Studio |
| 3 | Fine-tune a smaller model on production agent traces to keep invoice assurance quality while cutting cost and latency | Sarah Perez, AI App Developer | Microsoft Foundry |
| 4 | Observe, onboard, and govern every agent across the enterprise | Carlos Slattery, Chief Technology Officer | Microsoft Agent 365 |
| 5 | Key takeaways and next steps | — | — |

### 💻 Technologies used

- Microsoft Foundry (Foundry IQ, fine-tuning, Foundry Agent Service)
- GitHub Copilot
- Microsoft Copilot Studio
- Microsoft Agent 365
- Microsoft Entra, Microsoft Purview, and Microsoft Defender

### 📚 Continue your learning

Pick your next step based on your learning style:

| Resource | What you'll get |
|----------|-----------------|
| **[Learn Microsoft Foundry](https://aka.ms/AITourFoundryIntro)** | Get started building AI apps and agents with Microsoft Foundry |
| **[Agent Academy](https://aka.ms/Agent-Academy)** | Learn to build agents with Microsoft Copilot Studio |
| **[Learn Agent 365](https://aka.ms/A365Learn)** | Learn to observe, govern, and secure agents with Microsoft Agent 365 |
| **[Microsoft Learn](https://learn.microsoft.com)** | Official documentation and guided learning paths on these topics |
| **[AI Tour 2027 Resource Center](https://aka.ms/aitour27-resource-center)** | Additional session repos and materials from AI Tour 2027 |
| **[Microsoft Foundry Community](https://aka.ms/MicrosoftFoundryDiscord-AITour27)** | Connect with other learners and experts in our Discord community |

### 🌟 Microsoft Learn MCP Server

<!-- Remove this section if the Microsoft Learn MCP Server is not relevant to the session. -->

The Microsoft Learn MCP Server gives your AI agent direct access to Microsoft's official documentation — grounded, up-to-date answers about the topics in this session.

**GitHub Copilot CLI** — Install with:

```shell
copilot plugin install microsoftdocs/mcp
```

**VS Code** — One-click install:  
[![Install in VS Code](https://img.shields.io/badge/VS_Code-Install_Microsoft_Learn_MCP-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect/mcp/install?name=microsoft-learn&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Flearn.microsoft.com%2Fapi%2Fmcp%22%7D)

For more information, visit the [Learn MCP Server repo](https://aka.ms/learnmcp).

### 👥 Content owners

<!-- TODO: Add yourself as a content owner
1. Change the src in the image tag to {your github url}.png
2. Change INSERT NAME HERE to your name
3. Change the github url in the final href to your url. -->

<table>
<tr>
    <td align="center">
        <sub><b>Dona Sarkar</b></sub><br />
            📢
    </td>
    <td align="center"><a href="http://github.com/amynic">
        <img src="https://github.com/amynic.png" width="100px;" alt="Amy Boyd"/><br />
        <sub><b>Amy Boyd</b></sub></a><br />
            <a href="https://github.com/amynic" title="talk">📢</a>
    </td>
    <td align="center">
        <sub><b>April Dunham</b></sub><br />
            📢
    </td>
    <td align="center">
        <sub><b>Bethany Jepchumba</b></sub><br />
            📢
    </td>
</tr></table>

### Deliver this session

Presenters and re-delivery partners can find the deck, recordings, presenter
notes, and delivery guidance in [`delivery-resources/`](delivery-resources/README.md).

### 🤝 Contributing

This project welcomes contributions and suggestions. Most contributions require you to agree to a Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us the rights to use your contribution. For details, visit [Contributor License Agreements](https://cla.opensource.microsoft.com).

When you submit a pull request, a CLA bot will automatically determine whether you need to provide a CLA and decorate the PR appropriately. Simply follow the instructions provided by the bot. You will only need to do this once across all repos.

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any questions or comments.

### ⚖️ Trademarks

This project may contain trademarks or logos for projects, products, or services. Authorized use of Microsoft trademarks or logos is subject to and must follow [Microsoft's Trademark & Brand Guidelines](https://www.microsoft.com/legal/intellectualproperty/trademarks/usage/general). Use of Microsoft trademarks or logos in modified versions of this project must not cause confusion or imply Microsoft sponsorship.

Any use of third-party trademarks or logos are subject to those third-party's policies.
