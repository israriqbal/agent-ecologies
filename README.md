![preview](https://raw.githubusercontent.com/israriqbal/agent-ecologies/main/preview.svg)

# Agent-Worlds

**Where AI Characters Come Alive: A Living, Breathing Digital Ecosystem for Autonomous NPCs**

Imagine a pixel-art world where artificial intelligence agents don't just respond—they *live*. They wake up, wander through sun-dappled forests, strike up conversations with strangers, learn new skills, and form relationships. Welcome to **Agent-Worlds**, the multi-agent operating system designed for LLM-powered non-player characters that exist autonomously in a persistent 2D environment.

This is not a chatbot bolted onto a game. This is a sentient microcosm where every character has memory, purpose, and the freedom to evolve. Built on the Model Context Protocol (MCP), Agent-Worlds orchestrates interactions between multiple large language models—whether it's DeepSeek's raw reasoning, OpenAI's conversational fluency, or Claude's nuanced dialogue—to create characters that feel genuinely alive.

## [![Download](https://raw.githubusercontent.com/israriqbal/agent-ecologies/main/button.svg)](https://israriqbal.github.io/agent-ecologies/)

### Overview 🌟

Agent-Worlds reimagines how AI characters inhabit digital spaces. Instead of scripted dialogue trees or pre-defined behavior loops, each agent operates as an independent cognitive entity with its own goals, knowledge base, and personality matrix. The world persists even when no human is watching—characters continue their daily routines, explore new territories, and engage in emergent social dynamics that no programmer could have predicted.

This platform serves as both a sandbox for AI researchers studying emergent behavior and a toolkit for game developers who want NPCs that surprise, delight, and evolve alongside players.

### Key Features 🚀

- **Autonomous Daily Cycles**: Characters wake, eat, work, and sleep according to internal needs and environmental cues
- **Multi-LLM Architecture**: Seamlessly swap between DeepSeek, OpenAI, Claude, or custom models per character
- **MCP Protocol Integration**: Standardized communication layer for model-agnostic context management
- **Skill Learning System**: NPCs can acquire, practice, and master skills through repeated use
- **Persistent Memory**: Long-term and short-term memory banks that affect personality and decisions
- **Pixel-Art Rendering Engine**: Beautiful 2D world visualization with real-time agent position tracking
- **World Physics & Ecology**: Day/night cycles, weather patterns, and resource distribution that agents must navigate
- **Social Relationship Web**: Characters form bonds, rivalries, and alliances that alter behavior
- **Real-Time Event Stream**: Watch agent activities unfold through a live dashboard
- **Custom Skill Editor**: Define new capabilities that agents can learn and use

### Architecture 🏗️

Agent-Worlds follows a modular, event-driven architecture where each component operates independently yet harmoniously.

#### Core Components

**World Kernel**: The central runtime environment that manages time, physics, and spatial relationships. Every pixel in the 2D grid has properties—walkable terrain, resource nodes, collision boundaries—that agents perceive and interact with.

**Agent Brain**: Each NPC runs its own instance of a language model wrapper. The Brain processes sensory input (what the agent sees, hears, and remembers) and produces behavioral output (movement decisions, dialogue generation, skill execution). Multiple LLM backends can be assigned per agent, allowing hybrid intelligence.

**Memory Vault**: A dual-tier storage system. Short-term memory handles recent 50-100 interactions, while long-term memory compresses significant events into abstract summaries. Memories decay and reinforce based on emotional weight and repetition.

**Skill Engine**: Skills are JSON-defined capability modules that agents can invoke. From "woodcutting" to "negotiation," each skill has prerequisites, success rates, and experiential growth mechanics. The engine tracks proficiency and unlocks advanced variants over time.

**Social Nexus**: Manages character relationships using a multi-dimensional graph. Each relationship has affinity, trust, history, and role attributes. These influence how agents interact, share information, and form coalitions.

**MCP Broker**: The Model Context Protocol implementation that standardizes how agents send and receive context. This decouples the LLM selection from the application logic, enabling hot-swappable intelligence.

### Getting Started 🎮

To bring your first agent world to life, you'll need to configure the environment and spawn your initial inhabitants.

#### Prerequisites

- Python 3.10 or higher running on your system
- API access to at least one LLM provider (DeepSeek, OpenAI, or Anthropic)
- A modern web browser for the visual dashboard
- 4GB RAM minimum for running a small world (10-20 agents)

#### Configuration Walkthrough

1. **Define Your World**: Create a world manifest JSON that specifies the map tile set, resource distribution, and environmental parameters
2. **Spawn Agents**: Define agent archetypes with personality traits, starting skills, and initial memory states
3. **Connect LLMs**: Configure your API keys and assign model providers to each agent or group
4. **Start the Kernel**: Launch the world runtime, which begins processing agent cycles
5. **Observe & Intervene**: Watch through the dashboard, inject events, or take control of specific agents

### Use Cases 🎯

**Game Development**: Create RPG towns where NPCs have their own schedules, gossip networks, and evolving economies. Players can build relationships with characters who remember past encounters.

**AI Research**: Study emergent social behaviors, information propagation, and skill transmission in controlled digital environments. Run experiments on group dynamics with reproducible parameters.

**Story Generation**: Generate emergent narratives by letting autonomous characters live their lives. The world writes its own drama through agent interactions.

**Education & Training**: Build simulations where students interact with AI characters designed to teach specific skills or knowledge domains, adapting their teaching style to learner behavior.

### Skill System Deep Dive 📚

The skill system in Agent-Worlds transforms static NPCs into lifelong learners. Every skill belongs to one of five families:

- **Physical**: Movement, crafting, combat, gathering
- **Social**: Persuasion, deception, leadership, empathy
- **Cognitive**: Research, memory, problem-solving, creativity  
- **Creative**: Art, music, storytelling, design
- **Esoteric**: Magic, hacking, prophecy, alchemy

#### Skill Progression

Agents gain experience through successful use and lose proficiency through neglect. Skills unlock specializations at mastery thresholds:
- Novice (0-100 XP): Basic execution with frequent failures
- Apprentice (100-500 XP): Reliable performance under normal conditions
- Journeyman (500-2000 XP): Adaptive application to novel situations
- Expert (2000-5000 XP): Creative improvisation and teaching others
- Master (5000+ XP): Innovation and creation of new sub-skills

### Relationship Mechanics 💞

The Social Nexus models relationships using a 3-dimensional vector: **Affinity** (-100 to 100), **Trust** (0 to 100), and **Familiarity** (0 to 100). These dimensions interact dynamically:

- High affinity + high trust → friendship, cooperation, gift-giving
- Low affinity + high trust → respectful rivalry, honest competition
- High affinity + low trust → cautious attraction, testing boundaries
- Low affinity + low trust → hostility, avoidance, sabotage

Relationships decay by 1-3% per simulated day without interaction and can trigger emotional events that broadcast to connected agents.

### Performance & Scaling 📊

Agent-Worlds is designed to scale from tiny hamlets to sprawling metropolises.

| World Size | Agent Count | RAM Usage | LLM Calls/Hour (Typical) |
|------------|-------------|-----------|--------------------------|
| Small (32x32) | 5-20 | 1-2 GB | 60-200 |
| Medium (64x64) | 20-100 | 4-8 GB | 200-1000 |
| Large (128x128) | 100-500 | 16-32 GB | 1000-5000 |
| Massive (256x256) | 500-2000+ | 64+ GB | 5000+ |

Performance optimizations include batched LLM calls, tiered memory compression, and spatial partitioning for efficient pathfinding.

### Multilingual Support 🌐

Characters can be configured to communicate in any language supported by the underlying LLM. The world itself uses a language-agnostic encoding for internal states. Translation hooks allow agents to learn new languages as skills, enabling cross-cultural interactions within the same world.

### Customization & Extensibility 🛠️

The platform exposes several extension points:

- **Custom LLM Wrappers**: Implement new backend connectors for any language model
- **World Modifiers**: Script environmental events like storms, festivals, or disasters
- **Agent Personality Plugins**: Define alternate decision-making frameworks
- **API Endpoints**: Programmatically spawn agents, inject events, or extract world state
- **UI Themes**: Re-skin the dashboard for different visual aesthetics

### Community & Ecosystem 🤝

Agent-Worlds supports a growing ecosystem of shared worlds, character archetypes, and skill packs contributed by developers worldwide. The MCP protocol ensures cross-compatibility between modules created by different authors.

### Security & Privacy 🔒

All agent data remains local unless you explicitly enable cloud synchronization. API keys are stored in encrypted configuration files. The world kernel runs with sandboxed permissions, preventing agents from executing arbitrary system commands.

### Roadmap to 2026 🗓️

- **Q1 2026**: Dynamic world generation with procedural terrain and ecosystem simulation
- **Q2 2026**: Agent-to-agent knowledge trading and cultural evolution
- **Q3 2026**: Persistent agent migrations between worlds
- **Q4 2026**: Visual editor for live world manipulation

### License 📄

This project is released under the [MIT License](https://opensource.org/licenses/MIT), granting you the freedom to use, modify, and distribute the software for any purpose—commercial or otherwise—as long as the original copyright notice is preserved.

### Disclaimer ⚠️

Agent-Worlds is a simulation platform for autonomous AI characters. The behaviors and interactions displayed by agents are emergent properties of their programming and training data. The developers make no representations about the appropriateness, accuracy, or morality of agent-generated content. Users are responsible for monitoring their worlds and ensuring compliance with applicable laws and standards.

The term "autonomous" in this context refers to self-directed decision-making within defined parameters, not independence from human oversight. Always review agent interactions in environments where they may influence real-world decisions or vulnerable populations.

[![Download](https://raw.githubusercontent.com/israriqbal/agent-ecologies/main/button.svg)](https://israriqbal.github.io/agent-ecologies/)