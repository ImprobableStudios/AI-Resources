# AI Resources Document

---

## Document Maintenance and Update Instructions

This document is designed to be a living resource that evolves over time as new AI projects, frameworks, tutorials, and guides become available. To maintain consistency and usefulness, follow these guidelines when updating the document:

1. **Categorize New Resources by Theme:**  
   Group new links into existing themes (e.g., Local AI Frameworks, AutoGen Ecosystem, Learning Resources). If a new theme emerges, create a new section.

2. **Summarize Each Resource Clearly:**  
   Provide a brief description of the resource’s purpose and usefulness. Highlight key features or unique aspects.

3. **Note Potential Issues:**  
   Identify if the resource might be outdated (e.g., references to older framework versions like AutoGen 0.2), poorly maintained (check last commit/activity), or niche in applicability.

4. **Cross-Reference Related Resources:**  
   Where relevant, link or mention related projects or guides within the document to help users navigate the ecosystem.

5. **Date and Version Awareness:**  
   Prioritize resources from 2024 onward for relevance. Always check if official documentation or tools have newer stable versions.

6. **Note Costs or Fees:**  
   For each resource, note if there is an associated cost, subscription fee, or if it is free/open-source. This helps users understand potential barriers to adoption.

7. **Keep the Summary Notes Updated:**  
   Adjust the summary notes section to reflect new trends, deprecated tools, or emerging best practices.

8. **Update the Document Timestamp:**  
    Always update the "Document last updated" date at the bottom to reflect the latest revision.

9. **Duplicate Links Handling:**  
    When adding new links, do NOT remove existing links. If a provided new link exactly duplicates an existing one, do not add it and report it as a duplicate. Existing links may be reorganized as needed. The same link may appear in multiple sections as cross-references.

10. **GitHub Repository Maintenance Check:**  
    For GitHub links, check the last commit date to assess maintenance status and note this in the entry.

---

## Theme 1: Local AI and AGI Examples & Frameworks

_These resources focus on local AI frameworks, self-hosted AGI projects, and tools for running models without cloud dependencies._

### [LocalAI-examples (mudler)](https://github.com/mudler/LocalAI-examples)  
A collection of examples demonstrating LocalAI usage. Useful for developers wanting to run AI models locally without cloud dependencies.  
**Notes:** Check for recent updates; local AI frameworks evolve fast, so some examples might rely on older versions. Free and open-source.

### [LocalAI](https://localai.io/)  
Official site for LocalAI, an open-source platform for running LLMs and generative models locally. Focuses on privacy, extensibility, and compatibility with OpenAI APIs.  
**Notes:** Free and open-source; some integrations or models may have their own licensing.

### [LocalAGI (mudler)](https://github.com/mudler/LocalAGI)  
A project focused on building AGI-like agents that run locally. Good for experimentation with autonomous AI agents on local machines.  
**Notes:** Verify maintenance status; local AGI is a rapidly evolving field. Free and open-source.

### [Agent-S (simular-ai)](https://github.com/simular-ai/Agent-S)  
An AI agent framework, likely for building specialized agents. Could be useful for modular AI workflows.  
**Notes:** Check for recent commits and community activity to assess maintenance. Free and open-source.

### [helix (helixml)](https://github.com/helixml/helix) / [tryhelix.ai](https://tryhelix.ai/)  
Helix is a framework/tool related to AI or machine learning with a focus on local AI agent development and orchestration. The website (tryhelix.ai) offers a user-friendly interface and tools for building and managing AI agents locally with emphasis on privacy and customization. It supports multi-agent workflows and integrates with popular LLMs.  
**Notes:** Actively maintained, open-source with free access; some advanced features may require registration or subscription. Strong focus on local deployment and privacy.

### [Open WebUI (open-webui)](https://github.com/open-webui/open-webui)  
An open-source web user interface for running local AI models with ease. Supports multiple backends and models.  
**Notes:** Free and open-source.

### [Mentals AI (turing-machines)](https://github.com/turing-machines/mentals-ai)  
An AI agent framework or toolkit. Needs further exploration for specific use cases.  
**Notes:** Free and open-source; check maintenance status.

### [OpenHands (All-Hands-AI)](https://github.com/All-Hands-AI/OpenHands?tab=readme-ov-file)  
A repository focused on open-source AI hands-on projects and tools. Useful for practical AI applications and learning.  
**Notes:** Free and open-source.

---

## Theme 2: AutoGen Framework and Magentic Ecosystem

_Covers Microsoft's AutoGen framework and the Magentic-One multi-agent system, with resources for learning, implementation, and extending capabilities._

AutoGen is an open-source framework developed by Microsoft designed to facilitate the creation of multi-agent AI applications. It enables developers to build complex workflows by orchestrating multiple AI agents that can communicate, collaborate, and perform tasks autonomously. AutoGen emphasizes modularity, scalability, and ease of use, making it a state-of-the-art platform for generative AI applications.

Magentic-One (often misspelled as "Magnetic" or "Magnetic-One") is a cutting-edge generalist multi-agent system developed by Microsoft Research that builds on the AutoGen framework. It represents a significant advancement in agentic AI systems, designed to autonomously solve complex, multi-step tasks across diverse domains such as web navigation, file management, coding, and data analysis.

### Magentic-One Overview

Magentic-One employs a modular multi-agent architecture led by a central Orchestrator agent that plans, tracks progress, and directs four specialized agents:

- **Orchestrator:** The lead agent responsible for task decomposition, planning, and managing other agents.
- **WebSurfer:** Controls a Chromium-based web browser to navigate, interact with, and extract information from web pages.
- **FileSurfer:** Manages local file system navigation and file reading.
- **Coder:** Writes and analyzes code, creating new artifacts based on information from other agents.
- **ComputerTerminal:** Executes code and system commands in a console shell.

This design allows Magentic-One to flexibly and efficiently handle open-ended tasks by delegating subtasks to specialized agents, enabling autonomous adaptation to dynamic environments.

### Key Features and Capabilities

- **Generalist Agentic System:** Magentic-One is designed to solve a wide range of real-world tasks that require multiple steps and diverse skills, moving beyond simple conversational AI to autonomous task completion.
- **Modular and Extensible:** Agents can be added, removed, or replaced without reworking the entire system, supporting easy customization and scalability.
- **Model-Agnostic:** While the default large language model (LLM) used is GPT-4o, Magentic-One supports heterogeneous models tailored to different agents' needs.
- **Robust Planning and Recovery:** The Orchestrator maintains a task ledger and progress ledger to plan, monitor, and re-plan tasks, recovering from errors autonomously.
- **Open Source:** Microsoft has released Magentic-One and its evaluation tool AutoGenBench as open-source, encouraging community collaboration and research.

### Evaluation and Safety

Magentic-One has demonstrated competitive performance on benchmarks such as GAIA, AssistantBench, and WebArena, showing state-of-the-art capabilities in multi-agent task completion. Microsoft emphasizes safety and responsible AI use, conducting red-teaming exercises and recommending human oversight to mitigate risks like unintended actions or misuse.

### Related Resources

- [Magentic-One Technical Report (PDF)](https://www.microsoft.com/en-us/research/wp-content/uploads/2024/11/MagenticOne.pdf)
- [Microsoft Research Article on Magentic-One](https://www.microsoft.com/en-us/research/articles/magentic-one-a-generalist-multi-agent-system-for-solving-complex-tasks/)
- [Microsoft Research Publication](https://www.microsoft.com/en-us/research/publication/magentic-one-a-generalist-multi-agent-system-for-solving-complex-tasks/)
- [Magentic UI Blog](https://www.microsoft.com/en-us/research/blog/magentic-ui-an-experimental-human-centered-web-agent/)
- [Magentic-One YouTube Presentation 1](https://www.youtube.com/watch?v=RUDZZLtB08w)
- [Magentic-One YouTube Presentation 2](https://www.youtube.com/watch?v=JT5basX6JSY)
- [Medium Article: Microsoft Magentic-One Multi-Agent Framework](https://medium.com/data-science-in-your-pocket/microsoft-magnetic-one-new-multi-ai-agent-framework-7fd151b81cd7)

### AutoGen and Magentic Together

Magentic-One is built on top of the AutoGen framework, leveraging its multi-agent orchestration capabilities to deliver a powerful, generalist AI system. AutoGen provides the modular infrastructure, while Magentic-One adds a sophisticated agent hierarchy and task management system to solve complex, real-world problems autonomously.

### Core AutoGen Resources

- [Getting Started with AutoGen Multi-Agent Workflow Tutorial](https://www.gettingstarted.ai/autogen-multi-agent-workflow-tutorial/)  
  Beginner-friendly tutorial for building multi-agent workflows with AutoGen. Free.

- [AutoGen Studio v0.4 - No-Code Tool (newsletter.victordibia.com)](https://newsletter.victordibia.com/p/autogen-studio-v04-a-no-code-tool)  
  Overview of AutoGen Studio v0.4, a no-code platform for multi-agent AI apps. Free tier available; advanced features may require subscription.

- [Microsoft's AutoGen Blog (e2b.dev)](https://e2b.dev/blog/microsoft-s-autogen)  
  Insights into Microsoft’s AutoGen framework. Free.

- [Getting Started with AutoGen (singhrajeev.com)](https://singhrajeev.com/2025/02/08/getting-started-with-autogen-a-framework-for-building-multi-agent-generative-ai-applications/)  
  Recent blog post introducing AutoGen for generative AI. Free.

- [AutoGen Projects and Examples (projectpro.io)](https://www.projectpro.io/article/autogen-projects-and-examples/1129)  
  Curated list of AutoGen projects and examples. Free.

- [Building a Team of Experts with Microsoft's AutoGen (glasswing.vc)](https://glasswing.vc/blog/building-a-team-of-experts-with-microsofts-autogen/)  
  Conceptual guide on building expert AI teams with AutoGen. Free.

- [AutoGen is Mindblowing - 4 Features (towardsai.net)](https://pub.towardsai.net/autogen-is-mindblowing-4-features-that-make-autogen-the-state-of-the-art-framework-for-creating-ai-c7eb997b58a5)  
  Highlights key AutoGen features. Free.

- [What is AutoGen? Full Guide (skimai.com)](https://skimai.com/what-is-autogen-our-full-guide-to-the-autogen-multi-agent-platform/)  
  Comprehensive guide to AutoGen. Free.

- [Microsoft AutoGen Official Docs](https://microsoft.github.io/autogen/stable/user-guide/agentchat-user-guide/index.html)  
  Official documentation for AutoGen stable release. Free.

- [Autogen Course (pdichone)](https://github.com/pdichone/autogen-course)  
  Free, open-source course with tutorials and projects.

- [Dream Team (Azure-Samples)](https://github.com/Azure-Samples/dream-team)  
  Microsoft Azure sample project demonstrating AutoGen multi-agent teams. Azure services may incur costs.

- [Autogen Beginner Course (tylerprogramming)](https://github.com/tylerprogramming/autogen-beginner-course)  
  Beginner’s course for AutoGen. Free.

- [Multiagent Systems with AutoGen (victordibia)](https://github.com/victordibia/multiagent-systems-with-autogen?tab=readme-ov-file)  
  Practical guide and code repo for multi-agent systems with AutoGen. Free.

---

### AutoGen Skills and Community Examples

- [Reddit: More Examples of AutoGen Skillz](https://www.reddit.com/r/AutoGenAI/comments/199lgy3/more_examples_of_autogen_skillz/)  
  Community-shared AutoGen skills and examples. Free.

- [autogen_skillz (csabakecskemeti)](https://github.com/csabakecskemeti/autogen_skillz)  
  Collection of AutoGen skills. Free.

- [autogen-studio-skills (aj47)](https://github.com/aj47/autogen-studio-skills)  
  Skills for AutoGen Studio. Free.

- [autogenstudio-skills (madtank)](https://github.com/madtank/autogenstudio-skills)  
  Additional AutoGen Studio skills. Free.

- [openai-autogen-dev-studio (ivangabriele)](https://github.com/ivangabriele/openai-autogen-dev-studio)  
  Development tools and skills for AutoGen. Free.

- [autogen-studio-teams (2acrestudios)](https://github.com/2acrestudios/autogen-studio-teams)  
  Team collaboration skills for AutoGen Studio. Free.

- [autogen-studio-research (gabrielle-barnes)](https://github.com/gabrielle-barnes/autogen-studio-research/tree/main)  
  Research-focused AutoGen Studio skills. Free.

---

## Theme 3: AI Agent Development Guides and Learning Resources

_Guides, tutorials, and community projects for building AI agents, integrating LLMs, and developing AI-driven workflows._

### LiteLLM
LiteLLM is a lightweight, efficient large language model framework designed to enable easy deployment and usage of LLMs on local machines or edge devices. It focuses on minimal resource consumption while maintaining strong performance, making it suitable for developers and researchers who want to experiment with LLMs without requiring heavy infrastructure. The project is open-source and actively maintained, with comprehensive documentation and a GitHub repository for code and community contributions.  

**Links:**  
- [LiteLLM Official Site](https://www.litellm.ai/)  
- [LiteLLM Documentation](https://docs.litellm.ai/docs/)  
- [LiteLLM GitHub Repository](https://github.com/BerriAI/litellm)  
**Notes:** Free and open-source; ideal for lightweight LLM applications and local deployments.

### AIlice
AIlice is an AI agent framework aimed at building collaborative AI workflows and multi-agent systems. It provides tools and abstractions to create, manage, and orchestrate AI agents that can work together to solve complex tasks. The framework is open-source and supported by an active community, including a dedicated Reddit forum for discussions, support, and sharing use cases. AIlice is useful for developers looking to build modular AI systems with agent collaboration.  

**Links:**  
- [AIlice GitHub Repository](https://github.com/myshell-ai/AIlice)  
- [AIlice Reddit Community](https://www.reddit.com/r/AIlice/)  
**Notes:** Free and open-source; community-driven with active support channels.

### LangManus
LangManus is a tool designed to enhance application development and AI automation by providing a streamlined interface and automation capabilities. It supports developers in integrating AI-driven workflows into their applications, improving productivity and enabling advanced automation scenarios. There are tutorials and guides available for installation, testing, and leveraging LangManus features, along with video demonstrations.  

**Links:**  
- [YouTube: LangManus Introduction and Demo](https://www.youtube.com/watch?v=3M_L3wUsNEw)  
- [Leveraging LangManus for Enhanced Application Development and AI Automation (medium.com)](https://medium.com/@pankaj_pandey/leveraging-langmanus-for-enhanced-application-development-and-ai-automation-02d3b05baaa2)  
- [How to Install and Test LangManus - Step-by-Step Guide (medium.com)](https://medium.com/@prabhudev.guntur/how-to-install-and-test-langmanus-a-step-by-step-guide-9185ea377a00)  
**Notes:** Free resources available; practical for developers interested in AI automation and app integration.

### [Building Local AI Agents from Scratch - Developer's Guide (devthink.ai)](https://devthink.ai/p/building-local-ai-agents-from-scratch-a-developer-s-guide-using-ollama)  
Step-by-step guide for building local AI agents using Ollama. Practical for developers wanting hands-on experience.  
**Notes:** Verify if Ollama and related tools are current. Free.

### [Open Source LLMs on Your Own Computer (manning.com)](https://www.manning.com/liveprojectseries/open-source-llms-on-your-own-computer)  
Live project series teaching how to run open-source large language models locally. Very useful for hands-on learning.  
**Notes:** Check for updates as LLMs evolve quickly. Paid course.

### [Magnetic LLM Guide (algotrading101.com)](https://algotrading101.com/learn/magentic-llm-guide/)  
Guide focused on Magnetic LLM, possibly for algorithmic trading or specialized LLM use. Niche but useful for specific applications.  
**Notes:** Confirm if Magnetic LLM is actively maintained. Free guide; Magnetic platform may have costs.

### [Awesome AI Agents (e2b-dev)](https://github.com/e2b-dev/awesome-ai-agents)  
A curated list of AI agent projects and tools. Useful for discovering new frameworks and applications.  
**Notes:** Free and open-source.

### [CrewAI (crewAIInc)](https://github.com/crewAIInc/crewAI)  
An AI agent framework for building collaborative AI workflows.  
**Notes:** Free and open-source.

### [Langflow Quickstart (docs.langflow.org)](https://docs.langflow.org/get-started-quickstart)  
A visual tool for building and managing LLM workflows.  
**Notes:** Free and open-source.

### [Haystack (deepset.ai)](https://haystack.deepset.ai/)  
An open-source framework for building NLP pipelines and search systems with LLMs.  
**Notes:** Free and open-source; enterprise options available.

### [Local LLM Coding Assistants and Tools](https://medium.com/@smfraser/how-to-use-a-local-llm-as-a-free-coding-copilot-in-vs-code-6dffc053369d)  
Guide on using local LLMs as coding assistants in VS Code.  
**Notes:** Free.

### [Local LLM Chatbot with Code Searches (deepgram.com)](https://deepgram.com/learn/local-llm-chatbot-that-can-run-code-searches)  
Tutorial on building a local LLM chatbot capable of code searches.  
**Notes:** Free.

### [Personal Copilot with Hugging Face (huggingface.co/blog/personal-copilot)](https://huggingface.co/blog/personal-copilot)  
Guide on building a personal AI copilot using Hugging Face tools.  
**Notes:** Free; some Hugging Face services may have paid tiers.

### [Visual Studio Code AI Toolkit (techcommunity.microsoft.com)](https://techcommunity.microsoft.com/blog/educatordeveloperblog/visual-studio-code-ai-toolkit-run-llms-locally/4163192)  
Microsoft's toolkit for running LLMs locally in VS Code.  
**Notes:** Free.

### [Self-Hosted LLM Coding Assistants (semaphore.io)](https://semaphore.io/blog/selfhosted-llm-coding-assistants)  
Overview of self-hosted coding assistants powered by LLMs.  
**Notes:** Free.

### [n8n Local LLM Integration (blog.n8n.io)](https://blog.n8n.io/local-llm/)  
Guide on integrating local LLMs with n8n workflow automation.  
**Notes:** Free.

### [Reddit: Starter Guide for Local LLaMA](https://www.reddit.com/r/LocalLLaMA/comments/16y95hk/a_starter_guide_for_playing_with_your_own_local_ai/)  
Community guide for running local LLaMA models.  
**Notes:** Free.

### [Udemy AI Engineering Courses (multiple)](https://www.udemy.com/course/the-ai-engineer-course-complete-ai-engineer-bootcamp/?couponCode=ST4MT20725G1)  
Various paid courses on AI engineering and LLM app development.  
**Notes:** Paid courses; discounts may be available.

### [ScienceDirect Article on AI Agents](https://www.sciencedirect.com/science/article/pii/S266682702400046X)  
Academic article discussing recent advances in AI agents.  
**Notes:** Access may require subscription or institutional access.

### [Slashdot Discussions on AI Agents and Assistants](https://slashdot.org/software/ai-agents/linux/)  
Community discussions on Linux AI agents and free AI assistants.  
**Notes:** Free.

### [LAION-5B Dataset (laion.ai)](https://laion.ai/blog/laion-5b/)  
Information on the LAION-5B open dataset for training large AI models.  
**Notes:** Free and open.

### [MCP Pipedream (mcp.pipedream.com)](https://mcp.pipedream.com/)  
Platform for building AI workflows and integrations.  
**Notes:** Freemium model.

### [What LLM to Use (continuedev)](https://github.com/continuedev/what-llm-to-use)  
A guide to choosing the right LLM for your needs.  
**Notes:** Free and open-source.

### [YouTube: Local LLM Tutorial](https://www.youtube.com/watch?v=yG5Pvk9Bkqk&list=WL&index=22)  
Video tutorial on working with local LLMs.  
**Notes:** Free.

### [AI (tylerprogramming)](https://github.com/tylerprogramming/ai)  
A collection of AI projects, tools, and experiments. Useful for developers exploring practical AI implementations.  
**Notes:** Free and open-source.

### [AI System Development: LLM, RAG, AI Workflow, Agent (codelink.io)](https://www.codelink.io/blog/post/ai-system-development-llm-rag-ai-workflow-agent)  
A blog post providing a practical overview of building AI systems using LLMs, retrieval-augmented generation (RAG), and agent workflows.  
**Notes:** Free.

### [arXiv:2506.10943](https://arxiv.org/pdf/2506.10943)  
A recent academic paper (June 2025) on advanced AI agent systems, architectures, or evaluation.  
**Notes:** Free to access; highly relevant for those seeking the latest research.

---

## Theme 4: Enterprise AI Agents and Platforms

_Enterprise-level AI agent platforms, frameworks, and research for deploying and managing large-scale multi-agent systems._

### [AgentSpace Enterprise Gallery (cloud.google.com)](https://cloud.google.com/agentspace/agentspace-enterprise/docs/agents-gallery)  
Google Cloud’s AgentSpace platform showcasing enterprise AI agents and workflows. Useful for organizations looking to deploy AI agents at scale.  
**Notes:** Enterprise platform; usage may incur costs.

### Google MASS (Multi-Agent System Search) Framework and Research

Google AI has introduced MASS, a new framework for optimizing multi-agent AI systems through improved prompt engineering and agent topologies. This research aims to enhance collaboration and efficiency among AI agents in complex workflows.

- [arXiv Paper: MASS Framework (arxiv.org)](https://arxiv.org/html/2502.02533v1)  
  Academic paper detailing the MASS framework for multi-agent system optimization. Free and open access.

- [Learnopoly Overview: Google AI MASS Research](https://learnopoly.com/google-ai-presents-the-mass-of-research-for-multi-agent-systems-a-new-frame-of-optimization-of-ai-agents-for-better-prompts-and-topologies/)  
  Summary and analysis of Google’s MASS research and its implications for AI agent design. Free.

- [MarkTechPost Article: Google AI Introduces MASS](https://www.marktechpost.com/2025/06/07/google-ai-introduces-multi-agent-system-search-mass-a-new-ai-agent-optimization-framework-for-better-prompts-and-topologies/)  
  News article covering the MASS framework and its potential impact on AI workflows. Free.

- [Google Cloud Blog: What Execs Want to Know About Multi-Agentic Systems](https://cloud.google.com/blog/products/ai-machine-learning/what-execs-want-to-know-about-multi-agentic-systems-with-ai)  
  Enterprise-focused blog post explaining multi-agent AI systems and their business value. Free.

- [YouTube: Google AI MASS Presentation](https://www.youtube.com/watch?v=UsB3BR0RdBA)  
  Video presentation on the MASS framework and multi-agent system optimization. Free.

---

## Theme 5: Model Context Protocol (MCP) Ecosystem

_Resources and tools for the Model Context Protocol (MCP), enabling integration and orchestration of AI agents in local and privacy-focused environments._

The Model Context Protocol (MCP) is an emerging standard and ecosystem for integrating, orchestrating, and automating AI agents and tools, especially in local and privacy-focused environments. Below are key resources and projects in the MCP space:

### [MCP Protocol Servers (modelcontextprotocol)](https://github.com/modelcontextprotocol/servers?tab=readme-ov-file)  
A collection of MCP server implementations for various platforms and use cases.  
**Notes:** Free and open-source.

### [MCP.so](https://mcp.so/)  
A platform and hub for MCP-based tools, integrations, and community resources.  
**Notes:** Free to use; some integrations may have costs.

### [MCP Pipedream (mcp.pipedream.com)](https://mcp.pipedream.com/)  
Platform for building AI workflows and integrations using MCP.  
**Notes:** Freemium model.

#### MCP-Related Tools and Integrations

- [applescript-mcp (peakmojo)](https://github.com/peakmojo/applescript-mcp): AppleScript integration for MCP.  
- [choturobo (vishalmysore)](https://github.com/vishalmysore/choturobo): MCP-based automation tool.  
- [mcp-server-commands (g0t4)](https://github.com/g0t4/mcp-server-commands): Command server for MCP.  
- [mcp-remote-macos-use (baryhuang)](https://github.com/baryhuang/mcp-remote-macos-use): Remote MacOS integration for MCP.  
- [mcp-server-deep-research (reading-plus-ai)](https://github.com/reading-plus-ai/mcp-server-deep-research): Research-focused MCP server.  
- [DesktopCommanderMCP (wonderwhy-er)](https://github.com/wonderwhy-er/DesktopCommanderMCP): Desktop command integration for MCP.  
- [mcp-server-email (Shy2593666979)](https://github.com/Shy2593666979/mcp-server-email): Email integration for MCP.  
- [iMCP (loopwork-ai)](https://github.com/loopwork-ai/iMCP): MCP implementation for iOS/macOS.  
- [mac_messages_mcp (carterlasalle)](https://github.com/carterlasalle/mac_messages_mcp): Mac Messages integration for MCP.  
- [mikrotik-mcp (jeff-nasseri)](https://github.com/jeff-nasseri/mikrotik-mcp): MikroTik router integration for MCP.  
- [todoist-mcp-server (abhiz123)](https://github.com/abhiz123/todoist-mcp-server): Todoist integration for MCP.  
- [kicad-mcp (lamaalrajih)](https://github.com/lamaalrajih/kicad-mcp): KiCad integration for MCP.  

**Notes:** All above are free and open-source unless otherwise noted.

### n8n AI Workflow Tools and Integrations
- [aichat (sigoden)](https://github.com/sigoden/aichat): AI chat integration for n8n.  
- [awesome-n8n (restyler)](https://github.com/restyler/awesome-n8n): Curated list of n8n resources and workflows.  
- [awesome-n8n-templates (enescingoz)](https://github.com/enescingoz/awesome-n8n-templates): Curated templates for n8n workflows.  
- [mcp-n8n-workflow-builder (salacoste)](https://github.com/salacoste/mcp-n8n-workflow-builder): MCP workflow builder for n8n.  
- [n8n-ai-workflows (lucaswalter)](https://github.com/lucaswalter/n8n-ai-workflows): Collection of AI workflows for n8n.  
- [n8n-free-templates (wassupjay)](https://github.com/wassupjay/n8n-free-templates): A collection of free n8n workflow templates.
- [n8n-mcp (czlonkowski)](https://github.com/czlonkowski/n8n-mcp): MCP integration for n8n workflow automation.  
- [n8n-mcp-serve (illuminaresolutions)](https://github.com/illuminaresolutions/n8n-mcp-serve): MCP server for n8n.  
- [n8n-nodes-comfyui (mason276752)](https://github.com/mason276752/n8n-nodes-comfyui): ComfyUI nodes for n8n.  
- [n8n-nodes-puppeteer (drudge)](https://github.com/drudge/n8n-nodes-puppeteer): Puppeteer nodes for n8n automation workflows.  
- [n8n-ultimate-scraper (Touxan)](https://github.com/Touxan/n8n-ultimate-scraper): Web scraping workflows for n8n.
- [n8n-workflow-builder (makafeli)](https://github.com/makafeli/n8n-workflow-builder): Tool for building n8n workflows.  
- [n8n-workflows (Zie619)](https://github.com/Zie619/n8n-workflows): Additional n8n workflows.
- [n8n_agent (kingler)](https://github.com/kingler/n8n_agent): AI agent integration for n8n.  
- [nodewriter (ivov)](https://github.com/ivov/nodewriter): AI writing assistant integrated with n8n.  
- [Rapid-Product-Development-with-n8n (PacktPublishing)](https://github.com/PacktPublishing/Rapid-Product-Development-with-n8n): Guide and examples for rapid product development using n8n.  
- [Stride-AI-Agents (joshpocock)](https://github.com/joshpocock/Stride-AI-Agents): AI agents for n8n workflows.  
- [ultimate-n8n-ai-workflows (oxbshw)](https://github.com/oxbshw/ultimate-n8n-ai-workflows): Advanced AI workflows for n8n.  
- [n8n-nodes-docker - npm](https://www.npmjs.com/package/n8n-nodes-docker): An npm package providing n8n nodes for Docker automation and integration.  
  **Notes:** Free and open-source; check for maintenance status and compatibility with the current n8n version.
- [venssy/n8n-nodes-docker](https://github.com/venssy/n8n-nodes-docker): GitHub repository for the `n8n-nodes-docker` package.

**Notes:** All above are free and open-source; check individual repos for maintenance status.

*For specific workflow templates and node packages, see Appendix: Useful n8n Workspaces and Nodes.*

---

## Theme 6: AI Coding Assistants and Development Tools

_Open-source AI-powered coding assistants, prompt libraries, and tools for software development productivity._

### [Kilo Code Documentation | Kilo Code Docs](https://kilocode.ai/docs/)
Official documentation for Kilo Code, an open-source AI coding assistant.
**Notes:** Free and open-source.

### [Kilo-Org/kilocode](https://github.com/Kilo-Org/kilocode)
GitHub repository for Kilo Code, an open-source AI coding assistant for planning, building, and fixing code.
**Notes:** Free and open-source; actively maintained.

### [jamesponddotco/llm-prompts](https://github.com/jamesponddotco/llm-prompts/)
A collection of prompts for enhancing productivity with large language models.
**Notes:** Free and open-source.

---

## Theme 7: AI Video Generation

_Tools and frameworks for AI-driven video generation and processing._

### [deepbeepmeep/Wan2GP](https://github.com/deepbeepmeep/Wan2GP)
A fast AI Video Generator for the GPU Poor. Supports Wan 2.1/2.2, Hunyuan Video, LTX Video and Flux.
**Notes:** Free and open-source.

---

## Theme 8: LLM Orchestration and AI Companion Development

_Resources for orchestrating LLM workflows and building AI companions using visual and programmatic tools._

### [Introducing Flowise: Your Ultimate Visual Tool for LLM Orchestration and AI Companion Development (medium.com)](https://medium.com/@slrk4444/introducing-flowise-your-ultimate-visual-tool-for-llm-orchestration-and-ai-companion-development-71887123458f)
An introduction to Flowise, a visual tool for building and managing LLM workflows and AI companions.
**Notes:** Free resource; Flowise itself is open-source.

### [n8n vs Flowise (oxylabs.io)](https://oxylabs.io/blog/n8n-vs-flowise)
A comparison article between n8n and Flowise for workflow automation and LLM orchestration.
**Notes:** Free resource.

### [Flowise Tutorial (datacamp.com)](https://www.datacamp.com/tutorial/flowise)
A tutorial on using Flowise for LLM orchestration.
**Notes:** Free resource; DataCamp may have paid courses.

### [PocketFlow (the-pocket.github.io)](https://the-pocket.github.io/PocketFlow/)
A project related to AI workflows or LLM orchestration.
**Notes:** Free and open-source; check for maintenance status.

---

## Theme 9: General AI Resources and Platforms

_A broad range of AI resources, including model directories, datasets, and search tools for AI integrations._

### [Models | OpenRouter](https://openrouter.ai/models?max_price=0)
A platform listing various AI models, with options to filter by price (e.g., free models).
**Notes:** Free models available; paid models may incur costs.

### [keywords:n8n-community-node-package - npm search](https://www.npmjs.com/search?q=keywords%3An8n-community-node-package)
Search results for n8n community node packages on npm. Useful for extending n8n functionalities.
**Notes:** Free and open-source packages.

---

## Appendix: Useful n8n Workspaces and Nodes

This appendix contains specific n8n Workspace and Node resources. In future updates to this document, such items should be placed here rather than in the main "n8n AI Workflow Tools and Integrations" section. This ensures the main section contains broader, more general resources, while this appendix remains the go-to location for precise workflow or node template references.

### Specific n8n Workflow Templates and Node Links

- [🔐🦙🤖 Private & Local Ollama Self-Hosted AI Assistant | n8n workflow template](https://n8n.io/workflows/2729-private-and-local-ollama-self-hosted-ai-assistant/)
- [Anthropic AI Agent: Claude Sonnet 4 and Opus 4 with Think and Web Search tool | n8n workflow template](https://n8n.io/workflows/4399-anthropic-ai-agent-claude-sonnet-4-and-opus-4-with-think-and-web-search-tool/)
- [News Research and Sentiment Analysis AI Agent with Gemini and SearXNG | n8n workflow template](https://n8n.io/workflows/5286-news-research-and-sentiment-analysis-ai-agent-with-gemini-and-searxng/)
- [🧠 Empower Your AI Chatbot with Long-Term Memory and Dynamic Tool Routing | n8n workflow template](https://n8n.io/workflows/3025-empower-your-ai-chatbot-with-long-term-memory-and-dynamic-tool-routing/)
- [Build Custom Workflows Automatically with GPT-4o, RAG, and Web Search | n8n workflow template](https://n8n.io/workflows/5024-build-custom-workflows-automatically-with-gpt-4o-rag-and-web-search/)
- [🤖 Create Your First AI Agent with Weather & Web Scraping (Starter Kit) | n8n workflow template](https://n8n.io/workflows/6035-create-your-first-ai-agent-with-weather-and-web-scraping-starter-kit/)
- [💥🛠️Build a Web Search Chatbot with GPT-4o and MCP Brave Search | n8n workflow template](https://n8n.io/workflows/3189-build-a-web-search-chatbot-with-gpt-4o-and-mcp-brave-search/)
- [🤖 Build an Interactive AI Agent with Chat Interface and Multiple Tools | n8n workflow template](https://n8n.io/workflows/5819-build-an-interactive-ai-agent-with-chat-interface-and-multiple-tools/)
- [keywords:n8n-community-node-package - npm search](https://www.npmjs.com/search?q=keywords%3An8n-community-node-package)

---
## Summary Notes on Outdated Content and Maintenance

- Projects referencing AutoGen versions before 0.4 (notably 0.2) may be outdated due to rapid framework evolution.
- Local AI and AGI projects should be checked for recent commits to ensure active maintenance.
- Tutorials and guides dated 2024 or later are more likely to be current and relevant.
- Official docs and no-code tools like AutoGen Studio v0.4 are highly recommended for up-to-date usage.
- Many resources are free and open-source; some platforms and courses have associated costs or subscription fees—these are noted where applicable.

---
*Document last updated: 2025-08-09*
