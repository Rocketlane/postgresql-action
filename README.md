# PostgreSQL GitHub Action

This [GitHub Action](https://github.com/features/actions) sets up a PostgreSQL database.

**Note**: this is a fork from [here](https://github.com/Harmon758/postgresql-action) since the maintainer of that repository seems to be inactive.

# Usage

See [action.yml](action.yml)

Basic:
```yaml
steps:
- uses: danielweller-swp/postgresql-action@v2
  with:
    postgresql version: '11'  # See https://hub.docker.com/_/postgres for available versions
    postgresql init scripts: 'init-db'
    postgresql conf: 'max_prepared_transactions=100'
```

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
