# Calo Approved Tools Register

This is the company-wide register of approved software tools at Calo — the tools we **allow and recommend** for writing code, hosting websites and apps, running agents, moving data, and keeping things running.

> 📌 **Getting access.** To use any tool listed here, or to request a tool that isn't on the list, speak to **Bohdan or Caspar**. Don't set up your own account — all accounts must be admin-managed company accounts, and Bohdan or Caspar will set one up and invite you.

## How this works

If you — or an AI agent building on your behalf — want a tool that is **not** on this list, do not sign up for it yourself. Speak to **Bohdan or Caspar**: we'll either point you to the approved equivalent or set up a managed company account and invite you.

### Why this matters

1. **Consistency.** New tech is exciting, but the cost of a choice can be paid decades after us. Every tech dimension (CI/CD, languages, databases) multiplies support cost: backing three tools per dimension means deep, ongoing expertise in all of them. We deliberately keep the list short.
2. **Expertise and support.** Not everyone has experience with a given tech, and peers take time to catch up. We only want tools we are experts in, with internal owners who can support them.
3. **Security and data management.** This protects our data. We encourage building, but not in a way that creates entry points for malicious hackers.
4. **IP ownership.** Everything you build at Calo should be owned by Calo, with access available at any time.
5. **Better options.** There may be a better alternative to what you found. The team can advise on the best tool for the job.
6. **People move on, cost compounds.** Today we work together, tomorrow we may not. We value company over team over me. Maintenance and support cost grows exponentially, not linearly, so fewer tools keeps us sane.

---

## AI Coding & AI Models

Tools where an AI model writes code, helps you build, or sits inside something you are building.

| Tool | What it is | Example use |
| --- | --- | --- |
| **Cursor (Anysphere) Pro** | A code editor with AI built in that writes and edits code for you | Describe a feature in plain English and Cursor writes the code |
| **Anthropic / Claude AI** | The company and product behind Claude, an AI model we build with | Powering an agent that reads emails and drafts replies |
| **OpenAI / ChatGPT** | A rival AI model provider, also used to build AI features | Running a chatbot that answers customer questions |
| **OpenRouter** | A single doorway to switch between many different AI models | Testing whether Claude or another model works better without rebuilding |
| **GitHub Copilot** | AI autocomplete and chat built into the code editor | Suggesting the next lines of code as an engineer types |
| **ChatPRD** | An AI tool that helps write product specs and requirements | Turning a rough idea into a clear brief engineers can build from |

## Languages & Code

The core programming languages and the place code lives.

| Tool | What it is | Example use |
| --- | --- | --- |
| **TypeScript** | Our main programming language for web and back-end code | Building the logic behind a website or an agent |
| **Python** | Our language for data, AI, and scripting work | Writing a script that processes data or runs an AI model |
| **GitHub / Git** | Where code is stored, version-controlled, and shared | Keeping every version of an agent's code so you can roll back |
| **GitHub Actions** | Runs tests and ships code automatically when changes are made (CI/CD) | Auto-testing and deploying a site whenever code is updated |

## Frontend

Tools for building what users see and click on.

| Tool | What it is | Example use |
| --- | --- | --- |
| **React / React Native** | The framework for building websites and mobile apps | Building the Calo app screens customers interact with |
| **Tailwind CSS** | A styling toolkit for making interfaces look good quickly | Styling a page without writing custom CSS from scratch |
| **Material UI** | A library of ready-made interface components | Dropping in pre-built buttons, forms, and menus |

## Hosting & Infrastructure

The servers and platforms where websites, apps, and agents actually run and live online. The bulk of our infra runs on AWS.

| Tool | What it is | Example use |
| --- | --- | --- |
| **Amazon Web Services (AWS)** | The cloud platform our infrastructure mostly runs on (see AWS stack below) | Hosting our databases, back-ends, and services |
| **Vercel** | A platform built to host websites and web apps quickly | Putting a Next.js website live on the internet in minutes |
| **Hetzner** | A cheaper, no-frills server provider based in Germany | Running an always-on agent on a low-cost server |
| **Railway** | A platform that hosts and runs apps and agents with minimal setup | Deploying an always-on agent so it runs continuously in the cloud |
| **Cloudflare** | Sits in front of websites for speed, security, and DNS | Protecting a site from attacks and speeding it up worldwide |
| **Google Cloud Console** | Google's cloud platform, used alongside AWS where needed | Running an agent's back-end or storing large datasets |

### AWS stack (within AWS)

The specific AWS services we standardise on. All sit under the company AWS account.

| Service | What it does in plain terms |
| --- | --- |
| **Lambda** | Runs small bits of code on demand without managing a server |
| **Fargate / ECS** | Runs containerised apps and services |
| **EKS** | Runs Kubernetes (managing lots of containers at scale) |
| **Step Functions** | Chains multiple steps into one automated workflow |
| **DynamoDB** | A fast NoSQL database for high-volume data |
| **RDS (PostgreSQL / Aurora)** | A traditional relational database |
| **S3** | Stores files and objects (images, backups, uploads) |
| **CloudFront** | Delivers content fast worldwide via a CDN |
| **ElasticSearch / OpenSearch** | Powers fast search across large datasets |
| **SQS / SNS / EventBridge** | Pass messages and events between services |
| **Cognito** | Handles user sign-up and login |
| **AppSync (GraphQL)** | Builds flexible APIs the front-end can query |
| **REST API** | Standard way for systems to talk to each other |
| **Serverless Framework / AWS CDK** | Define and deploy infrastructure as code |
| **Amplify** | Quickly connects front-end apps to AWS back-ends |
| **TypeORM** | Lets code talk to databases without raw SQL |
| **Secrets Manager** | Stores passwords and API keys securely |
| **Route53** | Manages domain names and DNS |
| **SES** | Sends transactional emails |
| **VPC** | The private network our services run inside |
| **WAF** | Firewall that blocks malicious web traffic |
| **Location Service** | Maps, geocoding, and location features |

## Automation & Agents

Tools that connect apps together and let tasks or agents run on their own.

| Tool | What it is | Example use |
| --- | --- | --- |
| **n8n** | A workflow automation tool for connecting apps and steps | Building an internal workflow that runs nightly to move data |
| **CrewAI** | A framework for building teams of AI agents that work together | Coordinating several agents to complete a multi-step task |
| **Make.com** | A visual tool that connects apps and automates workflows | A new order comes in and is auto-logged with a Slack alert |
| **Activepieces** | An open-source automation tool, similar to Make | Building an internal workflow that runs nightly to clean data |
| **Apify** | A platform that scrapes data from websites at scale | Pulling competitor pricing off the web automatically each day |
| **Airtable** | A spreadsheet-database hybrid that often powers automations | Holding structured data that an automation reads and writes to |
| **LangGraph** | A framework for building AI agents and their workflows | Proposed agent-building framework (alongside CrewAI). Eng to confirm which is standard |

## Databases & Data Tools

Tools for storing, moving, transforming, and visualising data.

| Tool | What it is | Example use |
| --- | --- | --- |
| **Pinecone (Vector DB)** | A database for AI that stores meaning, not just text, so agents can recall things | Letting an agent search company knowledge by meaning, not keywords |
| **dbt Cloud** | Cleans and transforms raw data into usable tables | Turning messy raw sales logs into a tidy table for reporting |
| **Metabase** | Turns data into charts and dashboards anyone can read | Building a live dashboard of daily revenue from our database |
| **Segment (Segment.io)** | A pipe that collects customer data and sends it where needed | Capturing a sign-up once and routing it to email, analytics, CRM |
| **dbdiagram** | A tool for sketching out how a database is structured | Mapping tables and how they link before an engineer builds them |

## APIs & Developer Services

Building blocks you plug into your own code to add a specific capability such as voice or messaging.

| Tool | What it is | Example use |
| --- | --- | --- |
| **ElevenLabs** | An API that turns text into realistic spoken voice | Giving an agent a natural-sounding voice for phone calls |
| **LiveKit** | Powers real-time voice and video between people or agents | Running a live voice conversation with an AI agent |
| **TYNTEC** | A messaging API for sending SMS and WhatsApp from code | An agent texting a customer an order confirmation |
| **2Chat** | Automate and send WhatsApp messages programmatically | Auto-replying to WhatsApp enquiries via a workflow |
| **Genderize.io** | A simple API that guesses gender from a first name | Personalising automated messages based on a name field |

## Monitoring & User Insight

Tools that watch live code and show how people use our products.

| Tool | What it is | Example use |
| --- | --- | --- |
| **Sentry** | Tracks errors and crashes in live apps and alerts you | Getting pinged the moment an agent throws an error in production |
| **HotJar** | Shows how people actually use your site via heatmaps and recordings | Watching where users click and drop off so you can fix the page |

---

_To get access to any tool above, or to propose a new one, speak to **Bohdan or Caspar**._
