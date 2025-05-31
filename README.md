# action-hugo

A composite action that builds a site with [Hugo](https://gohugo.io).

This repository is not meant to be referenced in third-party workflows; please fork the repository if you would like to use it in your project.

## Inputs

| Name              | Description                           | Default      |
| ----------------- | ------------------------------------- | ------------ |
| hugo_environment  | The hugo build environment.           | "production" |
| hugo_version      | The hugo version to use.              | "0.145.0"    |
| sass              | Whether to install dart sass.         | "false"      |
| working_directory | The working directory for the action. | "."          |

## Examples

```
jobs:
  hugo:
    runs-on: ubuntu-latest
    steps:
      - uses: lojoja/action-hugo@main
        with:
          hugo_environment: "development"
          hugo_version: "0.145.0"
          sass: "true"
```

## License

action-hugo is released under the [MIT License](./LICENSE)
