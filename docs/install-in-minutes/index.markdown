---
layout: content
title: Superexpert.AI Installation Walkthrough
tag: Docs
heading: Superexpert.AI Installation Walkthrough
subheading: Quickly set up Superexpert.AI locally from GitHub

---
<article>
{% capture markdown_content %}

# Installation Walkthrough: Set Up Superexpert.AI in Minutes

This walkthrough will guide you through setting up the Superexpert.AI platform on your local machine. Follow these simple steps to get your AI agent up and running in minutes!

## Prerequisites

Make sure you have the following installed:
- **Node.js** (18.18 or later)
- **PostgreSQL**
- **pgvector** (required for vector embeddings)

---

## Step 1 — Install Node.js

1. Check if you have Node.js installed by running:
```bash
node -v
```
2. If Node.js is not installed, download it from [nodejs.org](https://nodejs.org/).

---

## Step 2 — Clone Superexpert.AI and Install Dependencies

1. Clone the repository:
```bash
git clone https://github.com/Superexpert/superexpert-ai.git
```

2. Navigate into the project directory and install dependencies:
```bash
cd superexpert-ai
npm install
```

---

## Step 3 — Set Up PostgreSQL

1. Check your PostgreSQL installation:
```bash
psql --version
```

2. If PostgreSQL is not installed, download it from [PostgreSQL.org](https://www.postgresql.org/).

3. Create the database:
```bash
psql
CREATE DATABASE superexpert_ai_db;
\q
```

4. Configure your database connection by creating a `.env` file in the project root:
```bash
DATABASE_URL=postgresql://username:password@localhost:5432/superexpert_ai_db
```
Replace `username` and `password` with your database credentials.

5. Migrate your database to set up the necessary tables:
```bash
npm run migrate
```

---

## Step 4 — Install pgvector 

pgvector enables vector embeddings, enabling RAG and greatly enhancing search capabilities.

Install via Homebrew:
```bash
brew install pgvector
```

For other installation methods, see [pgvector's GitHub page](https://github.com/pgvector/pgvector).

---

## Step 5 — Run Superexpert.AI Locally

Start your Superexpert.AI instance:
```bash
npm run dev
```

Open your browser and navigate to [http://localhost:3000](http://localhost:3000). You should see your Superexpert.AI instance up and running! Click the **Register** link at the botto of the Login page to create a new account.

![Working Superexpert AI](superexpert-ai-working.png)
*Figure 1: Superexpert.AI running locally.*

Your local Superexpert.AI installation is now ready! Start creating AI agents and tasks tailored to your project's needs.

{% endcapture %}
{{ markdown_content | markdownify }}

</article>

If you encounter any issues walkthrough, please post a message to the [discussions forum](https://github.com/Superexpert/superexpert-ai/discussions).

