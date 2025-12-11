# DLENSAI Investor – Phase 1 Spotlight Generator**

Backend Script for Generating DLENS v16_1 Disruptor Spotlight Reports

This repository contains the Phase 1 Deliverable for the DLENSAI Investor project:
a working backend script that generates a DLENS v16_1 Disruptor Spotlight using the OpenAI API and the official DLENS Master Prompt.

The script produces a full HTML Spotlight report following the TSLA v16_1 Gold Standard template as closely as possible.

# What This Repo Contains
```
node_modules
/prompts
   └── DLENSAI_Spotlight_MasterPrompt_v1_for_API.txt    # DLENS v16_1 Spotlight prompt
spotlight.js                                            # Main generator script
package-lock.json                                       # Dependencies
package.json                                            # Dependencies
README.md                                               # This file
```
# How to Run the Spotlight Generator
## 1. Clone the repository or Download the File
```
git clone 
cd dlenesai-spotlight
```
## 2. Install dependencies
```
npm install
```
## 3. Create your .env file 
```
.env
```

## Then edit .env and fill in:
```
OPENAI_API_KEY=your_openai_key_here
OPENAI_ORG_ID=your_openai_org_id
OPENAI_PROJECT_ID=your_dlenesai_project_id
OPENAI_MODEL=gpt-4.1    # or the current required model
```

## Run the Spotlight Script
```
node spotlight.js <TICKER> <TERM_YEARS>
```
## Example 
```
node spotlight.js TSLA 10
```
## This outputs: Remember you need to wait until it will show the HTML
### example: DELENS_SPOTLIGHT_TSLA_10y_via_API.html
