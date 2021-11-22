# GraphQL @connection

## Serverless

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

## AWS Amplify

Its a set of purpose-built tools and services that makes it quick and easy for front-end web and mobile developers build full-stack applications on AWS and support the popular languages.

## API (GRAPHQL) Directives

Its provided by the Amplify CLI to enhance the Schema with additional capabilities.

### Amplify-provided directives

* @model: Defines top level object types in your API that are backed by Amazon DynamoDB
* @key: Configures custom index structures for @model types
* @auth: Defines authorization rules for your @model types and fields
* @connection: Defines 1:1, 1:M, and N:M relationships between @model types
* @function: Configures a Lambda function resolvers for a field
* @http: Configures an HTTP resolver for a field
* @predictions: Queries an orchestration of AI/ML services such as Amazon Rekognition, Amazon Translate, and/or Amazon Polly
* @searchable: Makes your data searchable by streaming it to Amazon OpenSearch
* @versioned: Defines the versioning and conflict resolution strategy for an @model type

### 3rd party directives

* @algolia
* @ttl
* @firehose
* @retain

## Add relationships between types

### @connection

The @connection directive enables the relationships between @model types.
and its supports relationships:

1. one-to-one
2. one-to-many  
3. many-to-one

### Definition

```java
directive @connection(keyName: String, fields: [String!]) on FIELD_DEFINITION
```

@connection is used to specify the relations between types.

## Resources used in this reading

1. [What is Serverless Architecture](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)
2. [AWS Amplify](https://aws.amazon.com/ar/amplify/)
3. [Directives](https://docs.amplify.aws/cli/graphql-transformer/directives/)
