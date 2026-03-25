# Example 1: Your First Conversation

> Time: ~10 minutes
> Goal: Get comfortable talking to Claude Code

## Setup

Make sure you're in the project folder and Claude Code is running:

```bash
cd ~/Desktop/claude-code-for-frode
claude
```

## Exercise 1: Ask a Question

Just type naturally:

```
What is this project? Read the files here and tell me what you find.
```

Claude will scan the directory, read the files, and give you a summary. Notice how it **actually reads your files** — this isn't a chatbot guessing.

## Exercise 2: Read and Analyze a File

```
Read the file sample-data/proteomics-sample.csv and give me a summary.
How many proteins are there? What are the sample groups? Any obvious patterns?
```

Claude will read the CSV, understand the structure, and give you a scientific summary. No uploading. No copy-pasting. It just reads it.

## Exercise 3: Ask a Follow-Up

This is where it gets powerful. Without re-explaining anything:

```
Which proteins show the biggest fold change between the control and treatment groups?
```

Claude remembers the context. It knows which file you're talking about. It builds on the previous answer.

## Exercise 4: Create Something

```
Write a Python script that reads the proteomics dataset, calculates fold changes,
and saves the results to a new CSV file called results.csv
```

Claude will write the script **and save it to your disk**. You now have a real, runnable Python file.

## Exercise 5: Run It

```
Run the script you just created and show me the output
```

Yes. It runs the code too.

## Exercise 6: Search the Web

```
Search PubMed for the 5 most recent papers on cerebrospinal fluid proteomics biomarkers in Alzheimer's disease
```

Claude will search the web and return current results — not something memorized from training data.

## What You Just Learned

- Claude Code reads your actual files
- It remembers context within a conversation
- It writes files to your computer
- It runs code
- It searches the web
- You didn't write a single line of code

**Next:** [02-research-assistant.md](02-research-assistant.md) — put Claude to work on real research tasks.
