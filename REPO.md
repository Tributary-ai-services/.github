# 🏗️ Tributary AI Services - Repository Guide

This document provides an overview of all repositories in the Tributary AI Services ecosystem, organized by functionality and purpose.

---

## 🔐 Core Security & Routing

### [tas-llm-router](https://github.com/Tributary-ai-services/tas-llm-router)
Secure routing service for LLM requests with built-in compliance scanning. Routes requests to major LLM providers while ensuring all generated images and completions meet security and compliance standards.

### [llm-invocation](https://github.com/Tributary-ai-services/llm-invocation)
Go client library for easy developer integration with tas-llm-router. Provides a simple, secure interface for invoking LLM services with automatic compliance checking.

---

## 📊 Data Processing & Compliance

### [audimodal](https://github.com/Tributary-ai-services/audimodal)
Advanced data ingestion pipeline (formerly "Kubernetes-Native Data Ingest") that supports multi-modal data ingestion while ensuring compliance and security. Scans all ingested data for security issues and maintains compliance standards throughout the ingestion process.

### [deeplake-api](https://github.com/Tributary-ai-services/deeplake-api)
API bindings and SDK wrappers for interfacing with DeepLake vector databases, providing fast and scalable retrieval capabilities for RAG systems.

---

## 🤖 Workflow & Agent Management

### [tas-workflow-builder](https://github.com/Tributary-ai-services/tas-workflow-builder)
Service for composing and managing multi-step AI workflows. Enables the creation of complex, automated processes that can orchestrate various AI services and data flows.

### [tas-agent-builder](https://github.com/Tributary-ai-services/tas-agent-builder)
Dynamic agent generation service that creates and deploys intelligent agents based on specific requirements and workflows.

### [tas-ML](https://github.com/Tributary-ai-services/tas-ML)
Comprehensive machine learning service supporting ML tasks, model training, inference, and ML pipeline orchestration within the Tributary ecosystem.

### [tas-live](https://github.com/Tributary-ai-services/tas-live)
Live streaming service for real-time output streaming from all TAS services. Provides real-time monitoring, live data feeds, and streaming analytics across the Tributary ecosystem.

---

## 🔌 Model Context Protocol (MCP)

### [tas-mcp](https://github.com/Tributary-ai-services/tas-mcp)
Advanced open implementation of the Model Context Protocol, featuring a server registry and discovery mechanism for orchestrating model context services.

### [tas-mcp-servers](https://github.com/Tributary-ai-services/tas-mcp-servers)
Collection of pre-built MCP servers that can be run locally, providing ready-to-use context services for various AI applications.

---

## 🖥️ Frontend & User Interfaces

### [aether](https://github.com/Tributary-ai-services/aether)
Modern web frontend application that provides a user-friendly interface for interacting with all Tributary AI Services. Offers comprehensive dashboards, workflow management, and system monitoring capabilities.

### [aether-be](https://github.com/Tributary-ai-services/aether-be)
Backend services supporting the Aether frontend, handling API requests, user management, and coordination between frontend and core Tributary services.

---

## 🚀 DevOps & Infrastructure

### [aether-shared](https://github.com/Tributary-ai-services/aether-shared)
DevOps and infrastructure configuration for all common services. Provides Docker and Kubernetes deployment configurations, making it easy to deploy and manage the entire Tributary ecosystem.

---

## 🏛️ Repository Architecture

The repositories are designed to work together as a cohesive ecosystem:

- **Core Services**: `tas-llm-router`, `audimodal`, `deeplake-api` form the foundation
- **Client Libraries**: `llm-invocation` provides easy integration for developers
- **Intelligence Layer**: `tas-workflow-builder`, `tas-agent-builder` add AI capabilities
- **Protocol Implementation**: `tas-mcp`, `tas-mcp-servers` enable context sharing
- **User Experience**: `aether`, `aether-be` provide the interface layer
- **Infrastructure**: `aether-shared` handles deployment and operations

Each repository focuses on a specific concern while maintaining interoperability through well-defined APIs and protocols.