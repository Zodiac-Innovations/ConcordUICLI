# ConcordUICLI

<https://github.com/Zodiac-Innovations/ConcordUICLI>

The executable in this repository is published from the corresponding Development repository.


## Editable shared starter template

`Templates/SharedApplication.swift.template` is downloaded by `concordui init` at project setup time. The executable does not embed the starter Swift application. Changes to this text file on `main` affect new projects without rebuilding the CLI. Existing applications retain their generated source.


## Project workflow (after the next CLI publication)

```bash
concordui init MyApp
cd MyApp
concordui apple create
concordui apple ide
```

`init` writes the shared project and downloads the editable starter below. The project `.info` file defaults to the public ConcordUI framework repository on `main`; edit `repo` and `branch` to use an experiment. The platform `create` command generates the native project, which you compile in the appropriate IDE. Re-run `create -d` to regenerate after changing the framework selection.
