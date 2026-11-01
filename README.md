# Fidelity Pesquisas Court-Search Refactoring Challenge

Colab notebook with the statement and the legacy Python scraper of a refactoring challenge.

## Context

Hiring challenge of Fidelity Pesquisas (2025).

The repository contains a single notebook, `Teste_Fidelity_Pesquisas.ipynb`, saved from Google Colab. It holds:

1. The challenge statement (in Portuguese): reorganize the provided script following good practices, improve the logic of its functions and its queries, and design the database in PostgreSQL based on a table model shown as an embedded image.
2. The provided script, unchanged: class `SPVAutomatico`, which reads pending searches from a MariaDB database, queries the TJSP e-SAJ public court portal (`esaj.tjsp.jus.br`) with Selenium and headless Microsoft Edge by CPF, RG or name, classifies the page as "nothing found", "criminal" or "civil", and writes the result back to the database.

No refactored version, PostgreSQL schema or other solution code is committed.

The solution is not included in this repository.

## Tech stack (of the provided script)

- Python 3 (Colab kernel)
- `selenium` (Edge WebDriver), `mariadb`, `tqdm`

There is no requirements file or pinned versions.

## Running locally

The provided script is not runnable as is: it needs a reachable MariaDB with the expected schema, a local `msedgedriver.exe` path and a valid database host.


## Notes

- The notebook also includes the instructions addressed to candidates; the contact e-mail addresses in it were replaced with example addresses.
- The provided script contains placeholder database credentials (user `usr_teste`) and an invalid private IP; they come from the original statement.
