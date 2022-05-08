<div align="center" id="top"> 
  <img src="./.github/app.gif" alt="Hellopmlops" />

  &#xa0;

  <!-- <a href="https://hellopmlops.netlify.app">Demo</a> -->
</div>

<h1 align="center">Hellopmlops Seldon Mlflow</h1>

<p align="center">
  <img alt="Github top language" src="https://img.shields.io/github/languages/top/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8">

  <img alt="Github language count" src="https://img.shields.io/github/languages/count/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8">

  <img alt="Repository size" src="https://img.shields.io/github/repo-size/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8">

  <img alt="License" src="https://img.shields.io/github/license/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8">

  <!-- <img alt="Github issues" src="https://img.shields.io/github/issues/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8" /> -->

  <!-- <img alt="Github forks" src="https://img.shields.io/github/forks/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8" /> -->

  <!-- <img alt="Github stars" src="https://img.shields.io/github/stars/{{YOUR_GITHUB_USERNAME}}/hellopmlops?color=56BEB8" /> -->
</p>

<!-- Status -->

<!-- <h4 align="center"> 
	🚧  Hellopmlops 🚀 Under construction...  🚧
</h4> 

<hr> -->

<p align="center">
  <a href="#dart-about">About</a> &#xa0; | &#xa0; 
  <a href="#sparkles-features">Features</a> &#xa0; | &#xa0;
  <a href="#rocket-technologies">Technologies</a> &#xa0; | &#xa0;
  <a href="#white_check_mark-requirements">Requirements</a> &#xa0; | &#xa0;
  <a href="#checkered_flag-starting">Starting</a> &#xa0; | &#xa0;
  <a href="#memo-license">License</a> &#xa0; | &#xa0;
  <a href="https://github.com/{{YOUR_GITHUB_USERNAME}}" target="_blank">Author</a>
</p>

<br>

## :dart: About ##

This Helm Chart deploys seldon deployment along with mlflow cron job to track changes between Mlflow and Seldon Deployments

## :sparkles: Features ##

:heavy_check_mark: Automated Deployment from Mlflow to Seldon
:heavy_check_mark: Feature 2;\
:heavy_check_mark: Feature 3;

## :rocket: Technologies ##

The following tools were used in this project:

- [Seldon-Core](https://docs.seldon.io/projects/seldon-core/en/latest/index.html)
- [Mlflow](https://www.mlflow.org/docs/latest/index.html)

## :white_check_mark: Requirements ##

Before starting :checkered_flag:, you need to have [Helm](https://helm.sh/docs/helm/helm_install/) and [istio](https://istio.io/latest/docs/setup/install/istioctl/)

## :checkered_flag: Starting ##

```bash

#Setup Seldon Core With istio/ambassador

$ helm install seldon-core seldon-core-operator \
    --repo https://storage.googleapis.com/seldon-charts \
    --set usageMetrics.enabled=true \
    --set istio.enabled=true \
    --namespace seldon-system
    
# Setup Mlflow

# Clone this project
$ git clone https://github.com/HelloMLOps/mlflow-seldon-demo

# Access
$ cd hellopmlops

# Install Helm chart
$ helm install mlflow-seldon  ./mlflow-seldon

```

## :checkered_flag: To Deploy New Version With Mlflow ##


## :memo: License ##

This project is under license from MIT. For more details, see the [LICENSE](LICENSE.md) file.


Made with :heart: by <a href="https://github.com/HelloMLOps" target="_blank">HelloMLOps</a>

&#xa0;

<a href="#top">Back to top</a>
