# ***Developing AI Agents using GenAI***

## ***1. Chain of Thought Prompting***

***What it is:***

>#### A prompting technique where the AI is guided to reason step by step before giving the final answer.

***How we use it in EvoDoc:***

***When parsing a prescription, the AI reasons like:***

- ***Step 1: Identify the medicine name.***

- ***Step 2: Identify the dosage and frequency.***

- ***Step 3: Generate a patient-friendly explanation.***

**Why:** $Ensures$ $accurate,$ $stepwise$ $extraction$ $and$ $explanation,$ $reducing$ $errors$ $in$ $complex$ $prescriptions.$

## ***2. Dynamic Prompting***

***What it is:***

>#### Prompts that adapt based on input, instead of being fixed.

***How we use it:***

- ***If the prescription contains new drug names or instructions, the prompt dynamically changes to include those details for better explanation.***

**Why:** $Makes$ $AI$ $responses$ $context-aware$ $and$ $accurate$ $for$ $any$ $prescription.$

## ***3. Embeddings***

***What it is:***

>#### Numerical vector representations of text used by AI to understand semantic meaning.

***How we use it:***

- ***Prescription text and drug information are converted into embeddings.***

- ***These embeddings allow the AI to find similar drugs, dosages, or instructions in the database.***

**Why:** $Enables$ $semantic$ $search$ $and$ $RAG$ $(Retrieval-Augmented$ $Generation)$ $without$ $relying$ $only$ $on$ 
$keyword$ $matching.$

## ***4. Function Calling***

***What it is:***

>#### LLMs can call pre-defined functions for structured tasks instead of generating free text.

***How we use it:***

- ***The AI calls functions like parse_drug_info() or generate_patient_explanation().***

- ***Ensures structured, safe, and predictable output.***

**Why:** $Prevents$ $hallucinations$ $and$ $standardizes$ $outputs$ $for$ $downstream$ $use.$

## ***5. Multi-shot Prompting***

***What it is:***

>#### Providing multiple examples in a prompt to teach the AI patterns.

***How we use it:***

- ***Show examples of previous prescriptions and their plain-English explanations.***

- ***AI learns to apply the same structure to new prescriptions.***

**Why:** $Improves$ $accuracy$ $and$ $consistency$ $of$ $explanations.$

## ***6. One-shot Prompting***

***What it is:***

>#### Providing only one example in the prompt to guide the AI.

***How we use it:***

***For simple prescriptions, a single example suffices to guide the AI.***

**Why:** $Saves$ $tokens$ $and$ $still$ $guides$ $AI$ $effectively$ $for$ $small$ $tasks.$
