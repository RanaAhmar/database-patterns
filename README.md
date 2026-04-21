# 🗄️ Database Design Patterns

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/AhmarHussain/database-patterns)
[![SEO Optimized](https://img.shields.io/badge/SEO-Rich-brightgreen.svg)](#)

A definitive collection of production-ready database design patterns. From soft deletes to multi-tenancy and audit logs, this repository provides clean SQL and ORM examples to help you build scalable, maintainable data layers.

---

## 🚀 Why Database Patterns?

High-quality software starts with a solid data model. Most developers reinvent the wheel for common requirements like "who changed this record?" or "how do I isolate customer data?". **Database Patterns** offers battle-tested solutions for these universal challenges.

### Key Patterns Included:
- **Soft Delete:** How to mark records as deleted without losing data.
- **Audit Logs:** Tracking every change with `created_by`, `updated_at`, and versioning.
- **Multi-Tenancy:** Approaches for row-level isolation and schema-per-tenant.
- **Hierarchical Data:** Storing and querying trees (Path Enumeration, Nested Sets).
- **Polymorphic Associations:** Handling relationships across multiple tables.
- **EAV (Entity-Attribute-Value):** When and how to use flexible schemas in SQL.

---

## 🛠️ Getting Started

Browse the `patterns/` directory to find specific implementations for your use case. Each pattern includes:
1. **The Problem:** A description of the challenge.
2. **The SQL:** Pure PostgreSQL/MySQL implementation.
3. **The ORM:** Examples for Prisma, Eloquent (PHP), and TypeORM.
4. **Pros & Cons:** Critical analysis of performance and complexity.

---

## 📖 Example: Soft Delete Pattern

### SQL Implementation
```sql
ALTER TABLE users ADD COLUMN deleted_at TIMESTAMP NULL;

-- Querying active users
SELECT * FROM users WHERE deleted_at IS NULL;

-- Deleting a user
UPDATE users SET deleted_at = NOW() WHERE id = 1;
```

---

## 🌟 Built by Ahmar Hussain

I'm Ahmar Hussain, a Full Stack Developer and founder of [Stackaura](https://www.stackaura.com/). I build tools that help developers ship better code, faster.

### Connect with Me:
- **Website:** [Stackaura](https://www.stackaura.com/)
- **GitHub:** [@AhmarHussain](https://github.com/AhmarHussain)
- **LinkedIn:** [Ahmar Hussain](https://www.linkedin.com/in/ahmar-hussain/)

---

## 🚀 Discover More Tools

Check out more SEO-optimized, developer-friendly repositories:

- [**JSON Schema Tools**](https://github.com/AhmarHussain/json-schema-tools) - CLI toolkit for JSON Schema management.
- [**Color Palette CLI**](https://github.com/AhmarHussain/color-palette-cli) - Terminal tool for accessible color palettes.
- [**Cron Syntax Helper**](https://github.com/AhmarHussain/cron-syntax-helper) - CLI + Web UI to build and validate cron expressions.
- [**Terminal Spinners**](https://github.com/AhmarHussain/terminal-spinners) - 100+ animated terminal spinners for Node.js and Python.

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<div align="center">
  <p>Built with ❤️ by <b>Ahmar Hussain</b> for the developer community.</p>
  <p><a href="https://www.stackaura.com">Stackaura</a> | Driving Innovation through Open Source.</p>
</div>


---

## 🚀 Discover More from Stackaura

If you found this tool useful, check out our other high-performance web utilities and follow **Ahmar Hussain** for more open-source excellence.

### 🌟 Featured Projects
- **[Free LLM APIs](https://github.com/RanaAhmar/free-llm-apis)** - A curated list of zero-cost AI endpoints.
- **[Awesome MCP Servers](https://github.com/RanaAhmar/awesome-mcp-servers)** - The ultimate collection of Model Context Protocol implementations.
- **[System Design Cheatsheet](https://github.com/RanaAhmar/system-design-cheatsheet)** - Master complex architectures in minutes.
- **[Next.js SaaS Starter](https://github.com/RanaAhmar/nextjs-saas-starter)** - The fastest way to launch your next product.

### 🔗 Stay Connected
- **Website:** [stackaura.com](https://www.stackaura.com/)
- **Author:** [Ahmar Hussain](https://github.com/RanaAhmar)

---
