---
title: "Updated DDL SQL"
---

## Simplified DDL SQL 

This DDL SQL is a greatly simplified version of the original (very elaborate!) data structure that I modelled in the summer. 

I figured that I need to learn to walk before I can run so although this excludes so many of the parameters and relationships that I used in my original design, it's much, much easier to setup for MVP/POCs etc.

It still includes the "core" elements of my design: prompts, outputs, custom assistant/agent configs, and context snippets.

 ## Schema

 ```sql
CREATE TABLE Outputs (
    id SERIAL PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    prompt_id INT REFERENCES Prompts(id) ON DELETE CASCADE,
    agent_id INT REFERENCES Agents(id) ON DELETE CASCADE,
    output TEXT NOT NULL,
    version INT DEFAULT 1, -- Versioning for outputs
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE Prompts (
    id SERIAL PRIMARY KEY,
    text TEXT NOT NULL,
    version INT DEFAULT 1, -- Versioning for prompts
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE Agents (
    id SERIAL PRIMARY KEY,
    name VARCHAR(255) NOT NULL UNIQUE,
    configuration TEXT NOT NULL,
    use_case VARCHAR(255),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE ContextSnippets (
    id SERIAL PRIMARY KEY,
    name VARCHAR(255) NOT NULL UNIQUE,
    snippet_text TEXT NOT NULL,
    use_case VARCHAR(255),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE PromptAgentLink (
    prompt_id INT REFERENCES Prompts(id) ON DELETE CASCADE,
    agent_id INT REFERENCES Agents(id) ON DELETE CASCADE,
    PRIMARY KEY (prompt_id, agent_id)
);

CREATE TABLE OutputContextSnippetLink (
    output_id INT REFERENCES Outputs(id) ON DELETE CASCADE,
    context_snippet_id INT REFERENCES ContextSnippets(id) ON DELETE CASCADE,
    PRIMARY KEY (output_id, context_snippet_id)
);

CREATE TABLE PromptContextSnippetLink (
    prompt_id INT REFERENCES Prompts(id) ON DELETE CASCADE,
    context_snippet_id INT REFERENCES ContextSnippets(id) ON DELETE CASCADE,
    PRIMARY KEY (prompt_id, context_snippet_id)
);

CREATE TABLE Tags (
    id SERIAL PRIMARY KEY,
    name VARCHAR(255) NOT NULL UNIQUE
);

CREATE TABLE OutputTagLink (
    output_id INT REFERENCES Outputs(id) ON DELETE CASCADE,
    tag_id INT REFERENCES Tags(id) ON DELETE CASCADE,
    PRIMARY KEY (output_id, tag_id)
);
```