# helm-charts

## How It Works

I set up GitHub Pages to point to the docs folder. From there, I can create and publish docs like this:

```
$ helm create mychart
$ helm package mychart
$ mv mychart-0.1.0.tgz docs
$ helm repo index docs --url https://hown3d.github.io/helm-charts/
$ git add -i
$ git commit -av
$ git push origin
```

From there, I can do a `helm repo add NAME https://hown3d.github.io/helm-charts/`
