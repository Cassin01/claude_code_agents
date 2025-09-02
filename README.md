# Claude Code Agents

A collection of specialized agents for comprehensive software development workflows using Claude Code. These agents work together to provide systematic code analysis, planning, implementation, and review capabilities.

## Overview

This repository contains five specialized agents designed to cover the complete software development lifecycle:

- **🔍 Code Analyzer** - Analyzes code quality, performance, and best practices
- **📋 Problem Analyzer Planner** - Breaks down complex problems into implementation plans  
- **🔨 Task Planner Implementer** - Plans and executes development tasks
- **📝 Code Reviewer** - Provides comprehensive code reviews
- **🎯 Task Executor** - Coordinates execution of multiple sequential tasks

## Agent Descriptions

### Code Analyzer (`code-analyzer.md`)
**Purpose**: Analyze existing code for quality, performance, and maintainability issues  
**Tools**: Read, Grep, Glob, Bash  
**Use Cases**:
- Code quality assessments
- Performance bottleneck identification
- Security vulnerability analysis
- Architecture compliance reviews

### Problem Analyzer Planner (`problem-analyzer-planner.md`)  
**Purpose**: Analyze complex problems and create detailed implementation plans  
**Tools**: Full tool access  
**Use Cases**:
- Feature requirement analysis
- System design and architecture planning
- Risk assessment and mitigation strategies
- Technical solution design

### Task Planner Implementer (`task-planner-implementer.md`)
**Purpose**: Break down tasks into steps and execute implementation  
**Tools**: Full tool access  
**Use Cases**:
- Feature development from concept to completion
- Code refactoring with systematic approach
- Complex implementation tasks requiring planning

### Code Reviewer (`code-reviewer.md`)
**Purpose**: Comprehensive review of completed code changes  
**Tools**: Full tool access  
**Use Cases**:
- Post-implementation code reviews
- Security and quality assessments  
- Maintainability analysis
- Best practices validation

### Task Executor (`task-executor.md`)
**Purpose**: Systematically execute multiple tasks in sequence  
**Tools**: Full tool access  
**Use Cases**:
- Multi-feature implementation projects
- Sequential task coordination
- Progress tracking across complex workflows

## Usage Patterns

### Single Task Development
```
Problem Analyzer Planner → Task Planner Implementer → Code Reviewer
```

### Multi-Task Projects  
```
Task Executor → (Task Planner Implementer → Code Reviewer) × N
```

### Code Quality Assessment
```
Code Analyzer (can be used independently or as part of review process)
```

## Agent Capabilities

### Go Development Focus
- Event-driven architecture patterns
- Proper error handling with `github.com/cockroachdb/errors`
- Testing with `testify` framework
- Database patterns with PostgreSQL/SQLC
- Dependency injection and interface usage

### Frontend Development
- React component design and patterns  
- State management best practices
- Performance optimization techniques
- TypeScript integration and type safety

### Quality Assurance
- Comprehensive testing strategies (unit, integration, E2E)
- Security vulnerability assessment
- Performance optimization analysis
- Code maintainability evaluation

## Technical Standards

All agents follow consistent standards:
- **Language**: English-only code and comments
- **Documentation**: Minimal but necessary comments
- **Architecture**: Event-driven orchestrator patterns
- **Testing**: Comprehensive coverage with proper mocking
- **Error Handling**: Context-aware error wrapping
- **Database**: Snake_case naming, plural tables

## Getting Started

1. Choose the appropriate agent based on your task type
2. Ensure your project has a `CLAUDE.md` file for project-specific context
3. Use agents in the recommended workflow patterns
4. Leverage the structured output formats for consistent results

## Agent Coordination

The agents are designed to work together seamlessly:
- **Task Executor** coordinates multiple implementations
- **Problem Analyzer Planner** provides strategic direction
- **Task Planner Implementer** handles tactical execution
- **Code Reviewer** ensures quality standards
- **Code Analyzer** provides ongoing quality assessment

Each agent maintains awareness of project context and follows established patterns for consistent, high-quality development outcomes.