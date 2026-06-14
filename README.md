# Knowing-Machine
A Machine that knows.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Do you know anything about it, machine?" \
  | uvx knowing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
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
knowing-machine -a multilogue.txt
```
Or:
```bash
knowing-machine multilogue.txt > response.txt
```
Or:
```bash
knowing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import knowing_machine
```
