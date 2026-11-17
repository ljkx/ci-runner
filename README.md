# ci-runner

Runs a command against a branch of a public repository on a free GitHub-hosted Linux runner
(4 vCPU, 16 GB), so builds and tests don't queue on a local machine. Dispatch it with
`gh workflow run run.yml -R ljkx/ci-runner -f repo=... -f ref=... -f label=... -f command=...`,
or with the `cloud-run.sh` helper that waits for the run and prints its log.
