# C Calculator

A beginner-friendly C calculator project demonstrating modular C programming, unit testing with `assert()`, Makefile-based builds, and GitHub Actions CI.

## Project Structure

```text
c-calculator/
├── src/
│   ├── calculator.h
│   ├── calculator.c
│   └── main.c
├── tests/
│   └── test_calculator.c
├── .github/
│   └── workflows/
│       └── ci.yml
└── Makefile
```

## Operations

- Addition
- Subtraction
- Multiplication
- Division
- Division-by-zero handling

## Build

```bash
make all
./calculator
```

## Run Tests

```bash
make test
```

The test suite checks addition, subtraction, multiplication, normal division, and division by zero.

## Clean Build Files

```bash
make clean
```

## GitHub Actions

The workflow in `.github/workflows/ci.yml` runs on pushes and pull requests targeting `main`. It checks out the repository, installs GCC and Make, builds the application with `make all`, and runs the tests with `make test`.
