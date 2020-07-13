---
title: Serverless Functions reference architectures
titleSuffix: Azure Example Scenarios
description: Learn about serverless reference architectures.
author: rogeriohc
ms.date: 06/22/2020
ms.topic: guide
ms.service: architecture-center
ms.subservice: reference-architecture
ms.custom:
- fcp
---
# Serverless Functions reference architectures

A reference architecture is a template of required components and the technical requirements to implement them. A reference architecture isn't custom-built for a customer solution, but is a high-level scenario based on extensive experience. Before designing a serverless solution, use a reference architecture to visualize an ideal technical architecture, then blend and integrate it into your environment.

## Common serverless architecture patterns

Common serverless architecture patterns include:
- Serverless APIs, mobile and web backends.
- Event and stream processing, Internet of Things (IoT) data processing, big data and machine learning pipelines.
- Integration and enterprise service bus to connect line-of-business systems, publish and subscribe (Pub/Sub) to business events.
- Automation and digital transformation and process automation.
- Middleware, software-as-a-Service (SaaS) like Dynamics, and big data projects.

<table>
<tr>
    <td style="width: 250px;">
        <h3>Web application backends</h3>
        <p>Retail scenario: Pick up online orders from a queue, process them, and store the resulting data in a database</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/web-app-backends.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Mobile application backends</h3>
        <p>Financial services scenario: Colleagues use mobile banking to reimburse each other for lunch. Whoever paid for lunch requests payment through a mobile app, triggering a notification on colleagues' phones.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/mobile-app-backends.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>IoT-connected backends</h3>
        <p>Manufacturing scenario: A manufacturing company uses IoT to monitor its machines. Functions detects anomalous data and triggers a message to the service department when repair is required.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/iot-connected-backends.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Conversational bot processing</h3>
        <p>Hospitality scenario: Customers ask for available vacation accommodations on their smartphones. A serverless bot deciphers requests and returns vacation options.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/conversational-bot-processing.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Real-time file processing</h3>
        <p>Healthcare scenario: The solution securely uploads patient records as PDF files. The solution then decomposes the data, processes it using OCR detection, and adds it to a database for easy queries.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/real-time-file-processing.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Real-time stream processing</h3>
        <p>Independent software vendor (ISV) scenario: A massive cloud app collects huge amounts of telemetry data. The app processes that data in near real-time and stores it in a database for use in an analytics dashboard.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/real-time-stream-processing.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Scheduled task automation</h3>
        <p>Financial services scenario: The app analyzes a customer database for duplicate entries every 15 minutes, to avoid sending out multiple communications to the same customers.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/automation-scheduled-tasks.png" width="550"/></td>
</tr>
<tr>
    <td style="width: 250px;">
        <h3>Extending SaaS applications</h3>
        <p>Professional services scenario: A SaaS solution provides extensibility through webhooks, which Functions can implement to automate certain workflows.</p>
    </td>
        <td style="vertical-align: middle;"><img src="./images/extending-saas-app.png" width="550"/></td>
</tr>
</table>

## Featured serverless reference architectures

The following featured serverless reference architectures walk through specific scenarios. See the linked articles for architectural diagrams and details.

### Serverless microservices
The [serverless microservices reference architecture](https://docs.microsoft.com/samples/azure-samples/serverless-microservices-reference-architecture/serverless-microservices-reference-architecture/) walks you through designing, developing, and delivering the Rideshare application by Relecloud, a fictitious company. You get hands-on instructions for configuring and deploying all the architectural components, with helpful information about each component.

### Serverless web application and event processing with Azure Functions
This two-part solution describes a hypothetical drone delivery system. Drones send in-flight status to the cloud, which stores these messages for later use. A web application allows users to retrieve the messages to get the latest device status.
- You can download the code for this solution from [GitHub](https://github.com/mspnp/serverless-reference-implementation/tree/v0.1.0).
- The article [Code walkthrough: Serverless application with Azure Functions](https://docs.microsoft.com/azure/architecture/serverless/code) walks you through the code and the design processes.

### Event-based cloud automation
Automating workflows and repetitive tasks on the cloud can dramatically improve a DevOps team's productivity. A serverless model is best suited for event-driven automation scenarios. This [event-based automation reference architecture](https://docs.microsoft.com/azure/architecture/reference-architectures/serverless/cloud-automation) illustrates two cloud automation scenarios: cost center tagging and throttling response.

### Multicloud with Serverless Framework
The [Serverless Framework architecture](https://docs.microsoft.com/azure/architecture/example-scenario/serverless/serverless-multicloud) describes how the Microsoft Commercial Software Engineering (CSE) team partnered with a global retailer to deploy a highly-available serverless solution across both Azure and Amazon Web Services (AWS) cloud platforms, using the Serverless Framework.

## More serverless Functions reference architectures

The following sections list other serverless and Azure Functions-related reference architectures and scenarios.

### General

- [Serverless application architectures using Event Grid](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/serverless-application-architectures-using-event-grid)
- [Serverless apps using Cosmos DB](https://azure.microsoft.com/solutions/architecture/serverless-apps-using-cosmos-db/)
- [Serverless event processing using Azure Functions](https://docs.microsoft.com/azure/architecture/reference-architectures/serverless/event-processing)
- [Serverless web application on Azure](https://docs.microsoft.com/azure/architecture/reference-architectures/serverless/web-app)
- [Serverless Asynchronous Multiplayer Reference Architecture](https://docs.microsoft.com/gaming/azure/reference-architectures/multiplayer-asynchronous-serverless)
- [Instant Broadcasting on Serverless Architecture](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/instant-broadcasting-on-serverless-architecture)
- [Building a telehealth system on Azure](https://docs.microsoft.com/azure/architecture/example-scenario/apps/telehealth-system)
- [Custom Data Sovereignty & Data Gravity Requirements](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/data-sovereignty-and-gravity)
- [Sharing location in real time using low-cost serverless Azure services](https://docs.microsoft.com/azure/architecture/example-scenario/signalr/)


### Web and mobile backend
- [An e-commerce front end](https://docs.microsoft.com/azure/architecture/example-scenario/apps/ecommerce-scenario)
- [Architect scalable e-commerce web app](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/scalable-ecommerce-web-app)
- [Improve scalability in an Azure web application](https://docs.microsoft.com/azure/architecture/reference-architectures/app-service-web-app/scalable-web-app)
- [Uploading and CDN-preloading static content with Azure Functions](https://docs.microsoft.com/samples/azure-samples/functions-java-push-static-contents-to-cdn/functions-java-push-static-contents-to-cdn/)
- [Cross Cloud Scaling Architecture](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/cross-cloud-scaling)
- [Social App for Mobile and Web with Authentication](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/social-mobile-and-web-app-with-authentication)

### AI + Machine Learning
- [Image classification for insurance claims](https://docs.microsoft.com/azure/architecture/example-scenario/ai/intelligent-apps-image-processing)
- [Personalized Offers](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/personalized-offers)
- [Personalized marketing solutions](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/personalized-marketing)
- [Speech transcription with Azure Cognitive Services](https://docs.microsoft.com/azure/architecture/reference-architectures/ai/speech-ai-ingestion)
- [Training a Model with AzureML and Azure Functions](https://docs.microsoft.com/samples/azure-samples/functions-python-azureml-azurefunctions-deeplearning/training-a-model-with-azureml-and-azure-functions/)
- [Customer Reviews App with Cognitive Services](https://docs.microsoft.com/samples/azure-samples/functions-customer-reviews/customer-reviews-cognitive-services/)
- [Enterprise-grade conversational bot](https://docs.microsoft.com/azure/architecture/reference-architectures/ai/conversational-bot)
- [AI at the Edge](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/ai-at-the-edge)
- [Mass ingestion and analysis of news feeds on Azure](https://docs.microsoft.com/azure/architecture/example-scenario/ai/newsfeed-ingestion)
- [HIPPA and HITRUST compliant health data AI](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/security-compliance-blueprint-hippa-hitrust-health-data-ai)
- [Intelligent Experiences On Containers (AKS, Functions, Keda)](https://github.com/mohamedsaif/IntelligentExperiences.OnContainers)

### Data and analytics
- [Application integration using Event Grid](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/application-integration-using-event-grid)
- [Mass ingestion and analysis of news feeds](https://docs.microsoft.com/azure/architecture/example-scenario/ai/newsfeed-ingestion)
- [Tier Applications & Data for Analytics](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/tiered-data-for-analytics)
- [Operational analysis and driving process efficiency](https://docs.microsoft.com/azure/time-series-insights/time-series-insights-update-use-cases#operational-analysis-and-driving-process-efficiency)

### IoT
- [Azure IoT reference (SQL DB)](https://docs.microsoft.com/azure/architecture/reference-architectures/iot-with-sql)
- [Azure IoT reference (Cosmos DB)](https://docs.microsoft.com/azure/architecture/reference-architectures/iot)
- [IoT using Cosmos DB](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/iot-using-cosmos-db)
- [Facilities management powered by mixed reality and IoT](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/facilities-management-powered-by-mixed-reality-and-iot)
- [Complementary Code Pattern for Azure IoT Edge Modules & Cloud Applications](https://docs.microsoft.com/samples/azure-samples/iot-edge-complementary-code/complementary-code-pattern-for-azure-iot-edge-modules--cloud-applications/)

### Gaming
- [Custom Game Server Scaling](https://docs.microsoft.com/gaming/azure/reference-architectures/multiplayer-custom-server-scaling)
- [Non-real Time Dashboard](https://docs.microsoft.com/gaming/azure/reference-architectures/analytics-non-real-time-dashboard)
- [In-editor Debugging Telemetry](https://docs.microsoft.com/gaming/azure/reference-architectures/analytics-in-editor-debugging)
- [Multiplayer Serverless Matchmaker](https://docs.microsoft.com/gaming/azure/reference-architectures/multiplayer-matchmaker-serverless)
- [Advanced leaderboard for large scale](https://docs.microsoft.com/gaming/azure/reference-architectures/leaderboard-non-relational#advanced-leaderboard-for-large-scale)
- [Relational Leaderboard](https://docs.microsoft.com/gaming/azure/reference-architectures/leaderboard-relational)
- [Content Moderation](https://docs.microsoft.com/gaming/azure/reference-architectures/cognitive-content-moderation)
- [Text Translation](https://docs.microsoft.com/gaming/azure/reference-architectures/cognitive-text-translation)
- [Text to Speech](https://docs.microsoft.com/gaming/azure/reference-architectures/cognitive-text-to-speech)
- [Gaming using Cosmos DB](https://docs.microsoft.com/azure/architecture/solution-ideas/articles/gaming-using-cosmos-db)

### Automation
- [Smart scaling for Azure Scale Set with Azure Functions](https://docs.microsoft.com/samples/azure-samples/azure-scale-set-smart-downscale/smart-scaling-for-azure-scale-set-with-azure-functions/)
