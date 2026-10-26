# Trusting-Machine
A machine that establishes trust relationship.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Trust this statement, machine!" \
  | uvx trusting-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install trusting-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
trusting-machine -a multilogue.txt
```
Or:
```bash
trusting-machine multilogue.txt > response.txt
```
Or:
```bash
trusting-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import trusting_machine
```
