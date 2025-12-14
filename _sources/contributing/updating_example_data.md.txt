# Updating the example data

Metadata for eHabitat's example `InferenceData` objects (which are loadable by {func}`~eHabitat.load_eHabitat_data`) is stored in the [`eHabitat_example_data`](https://github.com/eHabitat-devs/eHabitat_example_data) repository.
This repo has been embedded into the `eHabitat` repo at `/eHabitat/data/example_data` using [git subtree](https://www.atlassian.com/git/tutorials/git-subtree) with the following command:

```bash
$ git subtree add --prefix eHabitat/data/example_data https://github.com/eHabitat-devs/eHabitat_example_data.git main --squash
```

When `eHabitat_example_data` is updated, the subtree within the `eHabitat` repo also needs to be updated with the following command:

```bash
$ git subtree pull --prefix eHabitat/data/example_data https://github.com/eHabitat-devs/eHabitat_example_data.git main --squash
```
