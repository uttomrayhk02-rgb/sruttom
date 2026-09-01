# AI Marketing Prompt Library

Reusable prompts for practical marketing workflows.

## Categories

- Google Ads
- Search-term analysis
- Conversion tracking
- GTM / GA4
- CRO
- Landing pages
- Competitor research
- Local-business research
- Reporting
- Content systems

## Prompt documentation standard

Every prompt should include:

```text
Problem
↓
Required Input
↓
Prompt
↓
Expected Output
↓
Example
↓
Version
```

## Example — Search Term Classifier

**Goal:** classify search terms by commercial relevance.

**Input:** a CSV or pasted list of search terms with campaign context.

**Output:**

| Search term | Intent | Relevance | Negative candidate | Reason |
|---|---|---|---|---|
| example | Commercial | High | No | Matches service intent |

The system should explain classifications instead of blindly applying them.
