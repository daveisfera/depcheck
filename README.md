[![Codacy Badge](https://app.codacy.com/project/badge/Grade/d1e91469175347b8afc72617f17efd9e)](https://app.codacy.com/gh/tj-actions/depcheck/dashboard?utm_source=gh\&utm_medium=referral\&utm_content=\&utm_campaign=Badge_grade)
[![CI](https://github.com/tj-actions/depcheck/workflows/CI/badge.svg)](https://github.com/tj-actions/depcheck/actions?query=workflow%3ACI)
[![Update release version.](https://github.com/tj-actions/depcheck/actions/workflows/sync-release-version.yml/badge.svg)](https://github.com/tj-actions/depcheck/actions/workflows/sync-release-version.yml)
[![Public workflows that use this action.](https://img.shields.io/endpoint?url=https%3A%2F%2Fused-by.vercel.app%2Fapi%2Fgithub-actions%2Fused-by%3Faction%3Dtj-actions%2Fdepcheck%26badge%3Dtrue)](https://github.com/search?o=desc\&q=tj-actions+depcheck+path%3A.github%2Fworkflows+language%3AYAML\&s=\&type=Code)

[![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?logo=ubuntu\&logoColor=white)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)
[![Mac OS](https://img.shields.io/badge/mac%20os-000000?logo=macos\&logoColor=F0F0F0)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)
[![Windows](https://img.shields.io/badge/Windows-0078D6?logo=windows\&logoColor=white)](https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idruns-on)

<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->

[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors-)

<!-- ALL-CONTRIBUTORS-BADGE:END -->

## depcheck

Analyze node project dependencies using [depcheck](https://github.com/depcheck/depcheck).

![sample](https://user-images.githubusercontent.com/17484350/153099924-30a3945a-4094-4a2d-a00e-4dc104644ef2.png)

## Usage

```yaml
...
    steps:
      - uses: actions/checkout@v4
      - name: depcheck
        uses: tj-actions/depcheck@v9
        with:
          ignores: 'eslint,babel-*'
```

*   Free software: [MIT license](LICENSE)

If you feel generous and want to show some extra appreciation:

[![Buy me a coffee][buymeacoffee-shield]][buymeacoffee]

[buymeacoffee]: https://www.buymeacoffee.com/jackton1

[buymeacoffee-shield]: https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png

## Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|                         INPUT                         |  TYPE  | REQUIRED |  DEFAULT  |                                 DESCRIPTION                                  |
|-------------------------------------------------------|--------|----------|-----------|------------------------------------------------------------------------------|
|       <a name="input_dir"></a>[dir](#input_dir)       | string |  false   |   `"."`   | The directory to run [depcheck](https://github.com/depcheck/depcheck#readme) |
| <a name="input_ignores"></a>[ignores](#input_ignores) | string |  false   |           |               Comma separated list of packages <br>to ignore                 |
| <a name="input_version"></a>[version](#input_version) | string |  false   | `"1.4.7"` |       Version of [depcheck](https://github.com/depcheck/depcheck/tags)       |

<!-- AUTO-DOC-INPUT:END -->

## Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->

|                            OUTPUT                             |  TYPE  |    DESCRIPTION     |
|---------------------------------------------------------------|--------|--------------------|
| <a name="output_exit_code"></a>[exit\_code](#output_exit_code) | string | depcheck exit code |

<!-- AUTO-DOC-OUTPUT:END -->

## Features

*   Runs dependency checks using a specified location.
*   Ignores specific packages.

## Credits

This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter).

## Report Bugs

Report bugs at https://github.com/tj-actions/depcheck/issues.

If you are reporting a bug, please include:

*   Your operating system name and version.
*   Any details about your workflow that might be helpful in troubleshooting.
*   Detailed steps to reproduce the bug.

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->

<!-- prettier-ignore-start -->

<!-- markdownlint-disable -->

<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://home.boidol.dev/"><img src="https://avatars.githubusercontent.com/u/652404?v=4?s=100" width="100px;" alt="Raphael Boidol"/><br /><sub><b>Raphael Boidol</b></sub></a><br /><a href="https://github.com/tj-actions/depcheck/commits?author=boidolr" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/daveisfera"><img src="https://avatars.githubusercontent.com/u/1686193?v=4?s=100" width="100px;" alt="Dave Johansen"/><br /><sub><b>Dave Johansen</b></sub></a><br /><a href="https://github.com/tj-actions/depcheck/commits?author=daveisfera" title="Code">💻</a> <a href="https://github.com/tj-actions/depcheck/commits?author=daveisfera" title="Documentation">📖</a> <a href="https://github.com/tj-actions/depcheck/pulls?q=is%3Apr+reviewed-by%3Adaveisfera" title="Reviewed Pull Requests">👀</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->

<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
