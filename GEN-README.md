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
