# Contributing

## Explantions

We do our best to follows [Diataxis Documentation Framework](https://diataxis.fr/).

## How-Tos

###  Release a new version of an action

1. Verify the `CHANGELOG.md` file is up-to-date.
2. Create a [New Release](https://github.com/erlef/gh-actions/releases/new)
    1. The "Tag" and "Release title" **MUST** be match the following pattern:

      ```text
      <Launch Stage>/<Actio Name>@v<SemVer>
      ```

      Eg: `stable/removal-acking@v1.0.0`

    2. The SemVer **MUST** match the latest version in the `CHANGELOG.md` file.
