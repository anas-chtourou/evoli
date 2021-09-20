# Evoli 🐈

Lulu Dans Ma Rue's technical test taht a candidate need to do to apply for a DevOps / Fullstack developer position 🤓

## Subject 📝

The subject of this technical test is to automate the deployment of this repository to a **Kubernetes cluster. which you will create**. This app should be configure to be deployed by using for .e.g a CI/CD pipeline. In order to help you, below is the diagram that you could inspire to create a pipeline.

<p align="center">
  <img src="workflow.jpg" alt="workflow" width="500"/>
</p>

An existing **Dockerfile** already exist in the repository. You can re-use it to deploy the app in the Kubernetes cluster.

## Deploy the evoli app tips

- You'll need to set an environment variable to the Kubernetes deployment. The value is

```yaml
env:
    name: ENV
    value: prod
```

- Unit test can be run with the command **cargo test**
- Lint can be run with the **cargo clippy** command. If you choose to use **github action** an existing actions already exist to do this steps
- The app is running on the port *3000*. For this technical test don't bother with the Ingress, you could just expose it with the LoadBalancer type of service

## Test your deployment

Should everything works fine. You should see a page with something like this:

<p align="center">
  <img src="example.png" alt="workflow" width="500"/>
</p>

## Tool constraint

You are *incite to use whatever tool* it seems to you necessary to resolve this technical test. We'll *focus* on the solutions that you'll bring to resolve this technical test.

## Duration of this test

The test has been designed to last for about 2~3 days.

## Questions

If you have any questions. Please contact me at marc.intha-amnouay@luludansmarue.org