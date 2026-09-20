# C++ transaction-processing exercise

This repository contains one small C++ program that reads account balances, processes transfer requests, and prints the final balances sorted by amount and then account ID.

Despite the repository name, the current code is not a complete digital-wallet application. It has no authentication, persistence, transaction history, input validation, or user interface.

## Build and run

```bash
g++ -std=c++17 -Wall -Wextra -pedantic "Module 1 project" -o wallet_exercise
./wallet_exercise
```

The program expects input in this form:

```text
N
user_id balance       # repeated N times
T
from_user_id to_user_id amount  # repeated T times
```

It prints `Success` or `Failure` for each transfer, followed by the final balances.

## Known limitations

- Negative transfer amounts are not rejected.
- Unknown account IDs are not handled explicitly.
- Balances use integers rather than a money type.
- There are no tests or persistence.

This is retained as a programming-fundamentals exercise and is not a flagship portfolio project.
