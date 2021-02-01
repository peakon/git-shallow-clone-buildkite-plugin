# Git Shallow Clone Buildkite Plugin

Sets `--depth` flag for git-clone and git-fetch commands.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: buildkite-agent pipeline upload
    plugins:
      - peakon/git-shallow-clone#v0.0.1:
          depth: 1
```

## Configuration

### `depth` (Optional, number)

Shallow clone `--depth` (default = 1).

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request
