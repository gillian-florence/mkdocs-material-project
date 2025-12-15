## Administrator Guide — Writing Sample

This section is a representative writing sample from my work on Salesforce-based solutions. It demonstrates how I structure administrator-facing documentation for complex, modular systems.

**You can jump directly into the sample here:**

- **[View the mkdocs sample](installation.md)**
- **[View the full PDF version](../assets/pdfs/admin-guide.pdf){:target="_blank"}**
- **[Download the full PDF version](../assets/pdfs/admin-guide.pdf){:download}**

> The PDF reflects how this guide is delivered to customers in production.

The sections below provide context on audience, structure, and authoring decisions for reviewers who want additional background.


## What This Sample Is

An **installation and configuration guide** for a modular Salesforce solution, where features can be enabled independently based on client needs.

Shared setup is documented once, followed by standalone, feature-specific sections. This reflects real implementation scenarios where not every client uses every feature.

## Audience

Written for:

- **Salesforce System Administrators** configuring and maintaining the solution  
- **Implementation and project teams** deploying it across different client environments  

The content assumes Salesforce admin experience and focuses on setup and system behaviour—not end-user training.

## How the Guide Is Structured

**Installation & Common Setup**

Covers baseline installation steps and prerequisites that apply regardless of which features are enabled.

**Feature-Based Sections**

Each feature is documented independently using a consistent structure:

- **Overview:** purpose and applicability  
- **Metadata:** objects, fields, flows, permission sets  
- **Configuration:** step-by-step setup  

This allows selective reading and keeps the guide maintainable as features evolve.

## Salesforce Alignment

The documentation follows Salesforce terminology and administrative conventions and references Salesforce Help where appropriate to support implementation and reinforce best practices.

## Authoring Context

The production guide is authored in Microsoft Word and published as a PDF. I maintain structured work-in-progress versions alongside hands-on testing to manage accuracy and change.

This portfolio version presents the same content in a docs-as-code format to demonstrate how it can be structured and maintained using modern documentation workflows.

