# Knowing-Machine
A machine that knows.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Are language models seeking the Truth, machine?" \
  | uvx knowing-machine \
    --provider-api-key=sk-proj-... \
    --github-token=ghp_... 
```

Or, with a local pip installation:
```bash
pip install knowing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
knowing-machine multilogue.txt
```
Or:
```bash
knowing-machine multilogue.txt new_turn.txt
```
Or:
```bash
cat multilogue.txt | knowing-machine
```
Or:
```bash
cat multilogue.txt | knowing-machine > tmp && mv tmp multilogue.txt
```
Or: 
```bash
(cat multilogue.txt; echo:"Theodotos: What do you think, Knowing-Machine?") \
  | knowing-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | knowing-machine
```
Or:
```bash
cat multilogue.txt new_turn.txt | knowing-machine >  tmp && mv tmp multilogue.txt
```
Or, if you have installed other machines:
```bash
cat multilogue.md | knowing-machine \
  | summarizing-machine | judging-machine > summary_judgment.md
```

Or use it in your Python code:
```Python
# Python
import knowing_machine
```
