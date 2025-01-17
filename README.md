# bop
# Set up

```shell
$ conda create -n bop --file conda-linux-64.lock
$ conda activate bop
$ poetry install --with=dev,gpu --no-root
```

# Dev

Only run if changes are made to the environment files.

To recreate the conda lock, after modifying conda.yaml:
```shell
pip install conda-lock
make conda-linux-64.lock
```

To recreate the poetry lock, after modifying pyproject.toml:
```shell
make poetry.lock