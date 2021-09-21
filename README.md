# Evoli 🐈

<p align="center">
  <img src="evoli.gif" alt="workflow" width="500"/>
</p>

Lulu Dans Ma Rue's technical test for a candidate for the DevOps / Fullstack developer position 🤓

## Subject 📝

The subject of this technical test is to automate the deployment of this repository to a **Kubernetes cluster which you will create**.

The app needs to be automated to allow developers to easily deploy their work on the Kubernetes cluster. You can use, for example, a CI/CD pipeline based on the diagram below.

### Sum-up of the subject

- Create a Kubernetes cluster
- Automate the deployment of this app

<p align="center">
  <img src="workflow.jpg" alt="workflow" width="500"/>
</p>

## Deploy the evoli app tips

- An existing **Dockerfile** already exists in the repository. You can re-use it to build the container
- You'll need to set an environment variable to the Kubernetes deployment. Below is the env setted in plain Kubernetes YAML spec

```yaml
env:
    name: ENV
    value: prod
```

- Unit test can be ran with the command **cargo test**
- Lint can be ran with the **cargo clippy** command. If you choose to use **github action** an existing action already exists to do this step
- The app is running on the **port 3000**.
- Don't bother with the Ingress. You can expose the app with the LoadBalancer type

## Test your deployment

Should everything work. Type the loadbalancer IP and you should see something similar to:

<p align="center">
  <img src="example.png" alt="workflow" width="500"/>
</p>

## Tool constraint

You are *invited to use whatever tool* it seems necessary to resolve this technical test. We'll *focus* on the solutions.

## Duration of this test

It's ok if you don't finish the test. My recommendation is not to spend more than 20 hours on it. Once again we're more interested in how you try to solve the technical issues.

## Questions

If you have any questions. Please contact me at marc.intha-amnouay@luludansmarue.org