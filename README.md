Some images leveraged by GitHub Actions have rate limit issues coming from DockerHub.  Using this repo to package these on ghcr


```bash
skopeo copy docker://repo/image:latest docker://ghcr.io/bdwyertech/dhub/image:latest --multi-arch all --dest-username bdwyertech --dest-password $GITHUB_API_KEY
```
