---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Superexpert.AI - Install in Minutes
---


# Superexpert.AI: Install in Minutes

**Walkthrough:** Set up Superexpert.AI locally by downloading it from GitHub.

## Step 1: Install Node.js

You'll need Node.js 18.18 or later. You can verify if you have Node.js installed by executing the following command in terminal:

```bash
node -v
```
If Node.js is not installed, download and install it from [nodejs.org](https://nodejs.org/).

## Step 2: Clone the Superexpert.AI GitHub repo and install dependencies

Clone the superexpert-ai repository by executing the following command in terminal:

```bash
git clone https://github.com/Superexpert/superexpert-ai.git
```

Switch into the root of the superexpert-ai folder and install all dependencies:

```bash
npm install
```


## Step 3: Setup PostgreSQL

You can check if you have PostgreSQL installed by executing the following command in terminal:

```bash
psql --version
```

If you don't have PostgreSQL installed then download and install it from [PostgreSQL.org](https://www.postgresql.org/){:target="_blank"}.

Next, create a new PostgreSQL database by accessing the PostgreSQL prompt:

```bash
psql
```

Create a database named superexpert_ai_db by executing the following command:

```bash
CREATE DATABASE superexpert_ai_db;
```

You can exit psql by entering "\q".

After creating the database, you need to add a connection string to your .env file
in the root of your Superexpert.AI project. Create a file named .env that contains the following connection string (replace username and password with your actual database credentials)):

```bash
DATABASE_URL=postgresql://username:password@localhost:5432/superexpert_ai_db
```
Finally, create all of the required Superexpert.AI database tables by executing the following command in Terminal
from the root of your Superexpert.AI project:

```bash
npm run migrate
```

## Step 4: Install pgvector

To support vector embeddings, you must install pgvector. The easiest way to install pgvector is with homebrew:

```bash
brew install pgvector
```

Other installation options are described at [https://github.com/pgvector/pgvector](https://github.com/pgvector/pgvector).



## Step 5: Run Superexpert.AI locally

To start the platform, run the following command:

```bash
npm run dev
```

Open a web browser and navigate to localhost:3000. You should see:

![Working Superexpert AI](superexpert-ai-working.jpg)

## Problems?

If you encounter any issues walkthrough, please post a message to the [discussions forum](https://github.com/Superexpert/superexpert-ai/discussions).

