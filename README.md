# SAP TechEd 2026

**Developer Garage — Agent Lab — App Space**  
**2026 SAP TechEd Berlin Dev Garage & Agent Lab**

A personal collection of hands-on learning notes, notebooks, and event screenshots from **SAP TechEd 2026 in Berlin**, with a focus on the **AI Track**, **SAP AI Core**, **agentic AI**, and **SAP Generative AI Hub orchestration**.

> **Project status:** Learning materials and a Google Colab adaptation are documented here. Successful execution of live SAP AI Core inference and LLM calls depends on valid service credentials and model availability. No completed tutorial or benchmark result is claimed unless explicitly documented.

## Event overview

The SAP Developer Center **App Space** organizes the Developer Garage activities into **11 tracks and 36 tutorials**, as shown in the event interface. The wider [official mission](https://developers.sap.com/tutorials/mission-2026-sap-teched-berlin-dev-garage-agent-lab) groups its **36 tutorials into 20 mission groups**. These are two different ways of organizing the same event learning resources.

### App Space tracks

| Track | Tutorials shown in App Space | Main focus |
| --- | ---: | --- |
| Joule Studio Keynote Demo | 1 | Joule Studio agent demo |
| Joule Studio | 8 | Building Joule agents |
| Joule Work | 2 | Agent-assisted workflows |
| Joule Studio with N8N | 1 | Workflow automation |
| Joule Studio Agent Extension | 1 | Extending existing agents |
| Joule Studio Command Line | 1 | Command-line agent development |
| ABAP | 4 | ABAP development |
| Integration | 5 | SAP integration capabilities |
| Agentic AI with CAP | 5 | CAP, MCP servers, and agents |
| **AI** | **2** | **Tabular AI and SAP AI Core** |
| Frontend | 6 | UI5 Web Components for React |

*Track counts and descriptions reflect the supplied SAP TechEd App Space screenshot.*

## AI Track — Google Colab lab

The AI Track includes two tutorials:

| Tutorial | Duration | Focus |
| --- | --- | --- |
| [AI #1 — Add Prior Labs TabPFN-3.5 Plus on SAP AI Core to your AI Agent](https://developers.sap.com/tutorials/ai-core-prior-labs-langgraph) | 60 min | Tabular regression/classification, REST inference, LangChain agent |
| AI #2 — Setup SAP AI Core Basic Trial | 45 min | SAP AI Core setup |

I adapted **AI #1** from a local Python / VS Code workflow into a **Google Colab notebook**, allowing experimentation directly in a browser.

### Architecture

```text
Google Colab
  ├── payload_data.py (shipment records and ground truth)
  ├── SAP AI Core OAuth authentication
  ├── TabPFN-3.5 Plus inference
  │     ├── Regression: DELAY_DAYS
  │     └── Classification: LATE (Yes/No)
  ├── LangChain agent + LLM (subject to access)
  │     └── Logistics operations summary
  └── Evaluation
        ├── Mean Absolute Error (MAE)
        └── Classification accuracy
```
