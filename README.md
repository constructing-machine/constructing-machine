# Constructing-Machine
A machine that constructs.

In order to launch it from the command line or as a Python subprocess:
```bash
echo "Theodotos-Alexandreus: Can you construct a scaffold here, machine?" \
  | uvx constructing-machine \
    --provider-api-key sk-proj-... \
    --github-token ghp_... 
```

Or, with a local pip installation:
```bash
pip install constructing-machine
```
Set the environment variables:
```bash
export PROVIDER_API_KEY="sk-proj-..."
export GITHUB_TOKEN="ghp_..."
```
Then:
```bash
constructing-machine -a multilogue.txt
```
Or:
```bash
constructing-machine multilogue.txt > response.txt
```
Or:
```bash
constructing-machine -a multilogue.txt > tmp && echo tmp > multilogue.txt
```

Or use it in your Python code:
```Python
# Python
import constructing_machine
```
