## Installation

```bash
git clone https://github.com/nk53/stanalyzer
cd stanalyzer/src/stanalyzer/tests
git submodule update --init inputs
```

## Usage

Run all tests like so:

```bash
cd stanalyzer/src/stanalyzer/tests  # if not already there
./test.sh
```

Then check the output in `results/` to see if it looks reasonable.

## Uninstallation

To remove the test files:

```bash
cd stanalyzer/src/stanalyzer/tests  # if not already there
git submodule deinit inputs
```
