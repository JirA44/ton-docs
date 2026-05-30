Here's an improved version of the bounty solution:

BOUNTY: [ DoraHacks ] TON Docs LLM Fuzz (4th week): 190 issues (3/26) ($100 on github)
DESCRIPTION: - Remove question mark from AI copilot heading
- Improve image alt text casing
- Add cd step before npm commands
- Clarify "upload it" destination for glossary

Improved Solution:

**370. Remove question mark from AI copilot heading**
```bash
Change the H2 to “How to take advantage of AI translation copilot” (no question mark) for consistency.
```
https://github.com/ton-community/ton-docs/blob/ee42357f5954f777d7ebd937b2683096da3699bf/docs/v3/contribute/localization-program/how-it-works.mdx?plain=1#how-to-take-advantage-of-ai-translation-copilot

**371. Improve image alt text casing**
```bash
Apply the following changes to all images in the documentation:
| Original Alt Text | Improved Alt Text |
| --- | --- |
| `projectId` | Project ID |
| `github-glossary` | GitHub glossary |

Search for `alt="projectId"` and replace with `alt="Project ID"`.
Search for `alt="github-glossary"` and replace with `alt="GitHub glossary"`.
```
https://github.com/ton-community/ton-docs/blob/ee42357f5954f777d7ebd937b2683096da3699bf/docs/v3/contribute/localization-program/how-it-works.mdx?plain=1#glossary

**372. Add cd step before npm commands**
```bash
Update the steps to:
```bash
cd ton-docs/
git clone https://github.com/ton-community/glossary.git
cd glossary/
npm i
npm run generate -- <glossary_name>
```
Replace `<glossary_name>` with the name of the glossary you want to generate.
```
https://github.com/ton-community/ton-docs/blob/ee42357f5954f777d7ebd937b2683096da3699bf/docs/v3/contribute/localization-program/how-it-works.mdx?plain=1#glossary

**373. Clarify "upload it" destination for glossary**
```bash
Update the instructions to:
### Step 1: Understand the upload process

When uploading your glossary, please use the `ton-docs` repository as the target location.

```bash
cd ton-docs/
npm run upload
```
Make sure you have set the correct environment variables for the upload process to work correctly.
```
https://github.com/ton-community/ton-docs/blob/ee42357f5954f777d7ebd937b2683096da3699bf/docs/v3/contribute/localization-program/how-it-works.mdx?plain=1#upload-process
```