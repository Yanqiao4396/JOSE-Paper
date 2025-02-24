# JOSE Paper


## Compilation

### Locally

Please run the following docker command to compile markdown into PDF locally.



```
docker run --rm \
    --volume $PWD:/data \
    --user $(id -u):$(id -g) \
    --env JOURNAL=joss \
    openjournals/inara
```

### GitHub Action

This repo contains an action to automatically run compilation on push

The PDF is available via the Actions tab in your project and click on the latest workflow run. The zip archive file (including the paper.pdf) is listed in the run’s Artifacts section.
