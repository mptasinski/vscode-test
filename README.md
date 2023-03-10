# Test-extension

Testing VSCode publish v0.0.1a

## Releasing

1. create branch from master with your changes
1. validate and then merge changes to master
1. github action will trigger and create "release vx.x.x" pull request with version bump and changelog [release.yml](./.github/workflows/release.yml)
1. merge release pr
1. another action will run after merging release pr. Action will create version tag, and publish package [publish.yml](./.github/workflows/publish.yml)
1. profit
