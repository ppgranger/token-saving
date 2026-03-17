# Examples

This directory contains example fixtures and scripts for demonstrating Token-Saver's compression capabilities.

## Fixtures

Realistic CLI output samples in `fixtures/`:

| File | Description |
|------|-------------|
| `large_git_diff.txt` | A 300-line git diff across 5 files with additions, deletions, and context |
| `pytest_output.txt` | A pytest -v run with 50 passing tests, 2 failures, and 1 warning |
| `terraform_plan.txt` | A terraform plan adding/changing/destroying 15 AWS resources |
| `npm_install.txt` | An npm install output with 80+ packages and deprecation warnings |
| `kubectl_pods.txt` | A kubectl get pods output with 50 pods across 6 namespaces |

## Running the Demo

```bash
python3 examples/demo.py
```

This processes each fixture through the compression engine and prints before/after stats. The output matches the data in the README hero table.

## Custom Processors

See `custom_processor/` for an example of how to write and install a user-defined processor.
