# Task 3: BMAD Creative Intelligence Suite

## Overview

Task 3 implements the BMAD (Business Model Architecture & Design) Creative Intelligence Suite, a comprehensive system for creative problem-solving, innovation strategy, and collaborative workflows. This installation combines core BMAD functionality with the Creative Intelligence Suite (CIS) module to provide advanced facilitation capabilities.

## Installation Details

- **BMAD Version**: 6.0.1
- **CIS Module Version**: 0.1.6
- **Installation Date**: February 19, 2026
- **IDE Support**: Windsurf

## Architecture

### Core Components

The system is built around a modular architecture with two primary modules:

#### BMAD Core Module
- **Version**: 6.0.1 (Built-in)
- **Purpose**: Core workflow orchestration and task execution
- **Features**: 
  - Advanced elicitation techniques
  - Brainstorming workflows
  - Party mode collaborative sessions
  - Editorial review tools
  - Document indexing and sharding

#### Creative Intelligence Suite (CIS)
- **Version**: 0.1.6 (External)
- **Source**: [bmad-creative-intelligence-suite](https://github.com/bmad-code-org/bmad-module-creative-intelligence-suite)
- **Purpose**: Specialized creative and strategic workflows
- **Features**:
  - Design thinking facilitation
  - Innovation strategy frameworks
  - Problem-solving methodologies
  - Storytelling and narrative crafting
  - Presentation design expertise

## Available Agents

The system includes 8 specialized agents:

### Core Agents
1. **BMad Master** (🧙) - Master task executor and workflow orchestrator
2. **Brainstorming Coach** (🧠) - Elite brainstorming specialist
3. **Creative Problem Solver** (🔬) - Systematic problem-solving expert

### CIS Agents
4. **Design Thinking Coach** (🎨) - Human-centered design expert
5. **Innovation Strategist** (⚡) - Disruptive innovation oracle
6. **Presentation Master** (🎨) - Visual communication expert
7. **Storyteller** (📖) - Master narrative strategist
8. **Creative Problem Solver** (🔬) - Master problem solver

## Workflow Capabilities

### Core Workflows
- **Brainstorming**: 36 techniques across 7 categories with multiple selection modes
- **Party Mode**: Multi-agent collaborative discussions
- **Advanced Elicitation**: Sophisticated information gathering techniques

### CIS Workflows
- **Design Thinking**: 5-phase human-centered design process
- **Innovation Strategy**: Business model innovation and competitive analysis
- **Problem Solving**: TRIZ, Theory of Constraints, and Systems Thinking
- **Storytelling**: 25 narrative frameworks for compelling stories

## Directory Structure

```
task3/
├── .windsurf/
│   └── workflows/           # WindSurf workflow definitions
├── _bmad/
│   ├── _config/            # Configuration files and manifests
│   ├── _memory/            # Session memory and preferences
│   ├── core/               # Core BMAD functionality
│   └── cis/                # Creative Intelligence Suite
└── _bmad-output/           # Generated outputs and session results
```

### Key Configuration Files
- `_bmad/_config/manifest.yaml` - Installation and module metadata
- `_bmad/_config/agent-manifest.csv` - Agent definitions and capabilities
- `_bmad/_config/files-manifest.csv` - Complete file inventory with hashes
- `_bmad/core/config.yaml` - Core module configuration
- `_bmad/cis/config.yaml` - CIS module configuration

## Usage Examples

### Basic Agent Invocation
```bash
# Start BMad Master
agent bmad-master

# Launch brainstorming session
agent brainstorming-coach
> brainstorm

# Begin design thinking process
agent design-thinking-coach
> design-thinking
```

### Workflow Execution
```bash
# Run brainstorming workflow
workflow brainstorming

# Execute design thinking with context
workflow design-thinking --data project-context.md

# Start innovation strategy session
workflow innovation-strategy
```

### Advanced Features
```bash
# Document indexing
task index-docs --directory ./docs

# Editorial review
task editorial-review-prose --file document.md

# Document sharding
task shard-doc --input large-document.md
```

## Memory and Persistence

The system maintains persistent memory across sessions:
- **Storyteller Memory**: Tracks narratives and story preferences
- **Session History**: Maintains conversation context and outcomes
- **User Preferences**: Customizes agent behavior and communication styles

## Integration Capabilities

### IDE Integration
- **Windsurf**: Full integration with workflow definitions and agent access
- **Real-time Collaboration**: Multi-agent sessions within the IDE environment

### External Integrations
- **Document Processing**: Support for various file formats and content types
- **Version Control**: Git integration for tracking changes and collaborations
- **Output Management**: Structured file organization for generated content

## Configuration Options

### Core Settings
```yaml
# _bmad/core/config.yaml
output_folder: "./bmad-outputs"
user_name: "User"
communication_language: "english"
```

### CIS Settings
```yaml
# _bmad/cis/config.yaml
output_folder: "./creative-outputs"
user_name: "User"
communication_language: "english"
```

## Best Practices

1. **Preparation**: Provide context documents for better results
2. **Objective Setting**: Define clear goals before starting workflows
3. **Process Trust**: Allow agent facilitation to guide discovery
4. **Documentation**: Capture insights and outputs systematically
5. **Energy Management**: Take breaks during extended sessions

## Troubleshooting

### Common Issues
- **Agent Loading**: Ensure all configuration files are present and valid
- **Workflow Execution**: Check CSV data files for technique libraries
- **Memory Issues**: Clear session memory if performance degrades
- **Output Generation**: Verify write permissions for output directories

### Support Resources
- Individual workflow README files in `_bmad/cis/workflows/`
- Agent documentation in respective agent directories
- Core module documentation in `_bmad/core/`

## Development and Extension

### Adding New Agents
1. Create agent definition in `_bmad/core/agents/` or `_bmad/cis/agents/`
2. Update `agent-manifest.csv` with new agent details
3. Configure agent personality and capabilities

### Custom Workflows
1. Design workflow structure in `_bmad/core/workflows/` or `_bmad/cis/workflows/`
2. Create technique libraries (CSV files) for workflow methods
3. Update workflow manifests and configuration

### Module Development
- Follow existing module structure patterns
- Implement configuration YAML files
- Create comprehensive documentation
- Test integration with core system

## Version History

- **v6.0.1** (Current): Core BMAD platform with CIS 0.1.6 integration
- Previous versions maintained in Git history

## License and Credits

This implementation combines:
- BMAD Core Platform (Built-in)
- Creative Intelligence Suite by BMAD Code Organization
- Community contributions and extensions

---

For detailed documentation on specific workflows or agents, refer to the respective README files in the `_bmad` directory structure.
