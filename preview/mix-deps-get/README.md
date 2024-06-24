# erlef/gh-actions/preview/mix-deps-get

Install dependencies with caching for Mix projects.

## References

### Usage

```yaml
jobs:
  Test:
    steps:
      # ...
      - name: Set up Elixir
        id: beam
        uses: erlef/setup-beam@v1
        with:
          version-file: .tool-versions
          version-type: strict
      - name: Install Dependencies
        uses: erlef/gh-actions/preview/mix-deps-get@main
        with:
          # We recommend to use `steps.beam.outputs` to get the version
          # of Elixir and Erlang/OTP to avoid version mismatch.
          elixir-version: ${{ steps.beam.outputs.elixir-version }}
          erlang-version: ${{ steps.beam.outputs.otp-version }}
          # Change the working directory to the root of the project where the
          # mix.exs file is located.
          # working-directory: ./myapp
```
