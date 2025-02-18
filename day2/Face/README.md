# Face Recognition

⏲️ _est. time to complete: 30 min._ ⏲️

## Here is what you will learn 🎯

In this challenge you will learn how to:

- how to create a Face API service in Azure
- how to connect you Face API service with your App
- how to pass the API key to you App using Github Secrets
- how to take a selfie 😉

*API - Application Programming Interface: A software intermediary that allows two applications to talk to each other*

### Further informative resources:

- [What is a Resource / Resource Group / Subscription?](https://docs.microsoft.com/azure/cloud-adoption-framework/govern/resource-consistency/resource-access-management)
- [Face API](https://azure.microsoft.com/services/cognitive-services/face/)
- [Regions and Availability Zones in Azure](https://docs.microsoft.com/azure/availability-zones/az-overview)
- [Github Encrypted secrets](https://docs.github.com/en/actions/reference/encrypted-secrets)

## Table of contents

- [Getting Started](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#getting-started)
- [Create Face Cognitive Service](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#create-face-cognitive-service)
- [Integrate Face Service Credential into Github Secret](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#integrate-face-service-credential-into-github-secret)
- [Run Frontend Pipeline again](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#run-frontend-pipeline-again)
- [Take Selfies! How old are you really? Play around!](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#take-selfies-how-old-are-you-really-play-around)
- [Overcharged? We got you covered](https://github.com/alumnitud/FemaleAIAppInnovationEcosystem/blob/main/day2/Face/README.md#overcharged-we-got-you-covered)

## Getting started

The first step in creating our Face API is to create a new resource.

*Azure Resource: In Azure, the term resource refers to an entity managed by Azure. For example, virtual machines, virtual networks, and storage accounts are all referred to as Azure resources.*

- Click the **big "+" symbol** on the main page
- Pick the category **"AI + Machine Learning"**
- Create a **Face** service.
![](./images/create-face.png)

## Create Face Cognitive Service

- Choose your **Subscription**
- Create a new **Resource Group** (A storage for multiple resources)
- Choose *West Europe* as **Region** (Location of datacenter where the service is deployed)
- Create a **unique name** and select the **Standard S0 Pricing Tier**.
![](./images/create-face-options.png)

## Integrate Face Service Credential into Github Secret

The API key is a unique identifier, which we will add to our code. By doing so, we can connect our code to the API and perform API calls.
![](./images/milligram-face-api-access-keys.png)

In Action Secrets you can store encrypted variables that you create in an organization, repository, or repository environment. These secrets are available to use in GitHub Actions workflows.
- Set the name and value similar to picture and replace the *xxxxxx* part with your values
- Add the secret
![](./images/vue-app-face-api-endpoint-secret.png)

![](./images/vue-app-face-api-key-secret.png)

## Run Frontend Pipeline again

Click on the frontend link displayed under the deploy step under your pipeline `https://<yourGithubHandle>.github.io/...`

Our frontend application should now have a new button with a selfie 🤩 symbol that allows us to take selfies and estimate how old we are.
These selfies will __not__ be saved and will __not__ appear on the timeline or News Feed.

## Take Selfies! How old are you really? Play around!

So go ahead and take at least 5 selfies and tell us how old you are in all of them.

Take also pictures of people who are around you and estimate their age, you might surprise them. 😁

That's a wrap for today! Congrats! 🥳🙏

Now we will make our app understand when we talk 🗣️ to our Milligram Social Media App. 


## Overcharged? We got you covered

Ask your coach if you did not succeed. We have you covered with a back up. ⚠️

### Use prepared Milligram Backend Service

Look at the prepared application with our pictures for you to play around [Milligram](https://codeunicornmartha.github.io/FemaleAIAppInnovationEcosystem/#/?stack-key=a78e2b9a).

:::tip
📝
  - Link1
  - Link2
:::

[◀ Previous challenge](../../day1/Application/README.md) | [🔼 Day x](../../README.md) | [Next challenge ▶](../Speech/README.md)
