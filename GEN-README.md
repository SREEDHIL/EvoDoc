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

## ***7. Stop Sequence***

***What it is:***

>#### A mechanism to tell the AI where to stop generating text.

***How we use it:***

- ***Ensures the AI stops after the prescription explanation, avoiding extra irrelevant text.***

**Why:** $Keeps$ $outputs$ $concise$ $and$ $usable$ $in$ $the$ $UI.$

## ***8. Structured Output***

***What it is:***

>#### Instead of plain text, AI outputs structured JSON or tables.

***How we use it:***

- ***Example: { "drug": "Paracetamol", "dosage": "500mg", "instructions": "Twice daily" }***

**Why:** $Easy$ $to$ $display$ $in$ $frontend$ $and$ $for$ $further$ $processing$ $or$ $storage.$

## ***9. System and User Prompt***

***What it is:***

>#### System prompt: Defines AI behavior.
>#### User prompt: The actual query or input.

***How we use it:***

- ***System prompt instructs AI to behave as a medical assistant.***

- ***User prompt contains the uploaded prescription text.***

**Why:** $RTFC$ $(Read$ $The$ $Fine$ $Context)$ $framework$ $ensures$ $AI$ $interprets$ $instructions$ $correctly.$

## ***10. Temperature***

***What it is:***

>#### Controls randomness in AI responses.

***How we use it:***

- ***Low temperature for precise, factual explanations (e.g., 0.2).***

- ***Higher temperature if you want slightly more natural or conversational text.***

**Why:** $Balances$ $accuracy$ $vs.$ $creativity.$

## ***11. Tokens and Tokenization***

***What it is:***

>#### Tokens are chunks of text AI reads or generates.

***How we use it:***

- ***Track token usage for cost management and optimization.***

- ***Ensure prompts + responses stay within model limits.***

**Why:** $Helps$ $manage$ $API$ $costs$ $and$ $model$ $efficiency.$

## ***12. Top K***

***What it is:***

>#### Selects the top K most probable next tokens for AI to choose from.

***How we use it:***

- ***Limits AI options to avoid irrelevant or unsafe outputs.***

**Why:** $Controls$ $diversity$ $while$ $maintaining$ $accuracy.$

## ***13. Top P***

***What it is:***

>#### Chooses tokens from the top cumulative probability mass P.

***How we use it:***

- ***Used with temperature and top K to fine-tune AI creativity vs. precision.***

**Why:** $Ensures$ $AI$ $doesn’t$ $hallucinate$ $while$ $still$ $producing$ $natural$ $text.$

## ***14. Vector Database***

***What it is:***

>#### Database storing embeddings for semantic search.

***How we use it:***

- ***Store prescription-related info and trusted drug data as vectors.***

- ***Query the database to fetch contextually relevant drug info during RAG.***

**Why:** $Provides$ $fast,$ $accurate,$ $and$ $context-aware$ $AI$ $retrieval.$
