# Advanced Usage

## Debugging for VS Code users

Create the file `.vscode/launch.json` with the following content:

```
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Micro GPT",
            "type": "python",
            "request": "launch",
            "program": "${cwd}/microgpt.py",
            "console": "integratedTerminal",
            "justMyCode": true,
            "args": ["test query"],
        }
    ]
}
```

Set the desired input arg ``<objective>`` and click "Run and Debug" in VS Code to start debugging.
