# Serverless and Amplify

## Serverless

Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls (Functions as a Service).

### The Serverless App

Serverless solution consist of the following:

1. Client Application
2. Web Server
3. Lambda functions (FaaS)
4. Security Token Service (STS)
5. User Authentication
6. Database

There are a lot of benefits for the Serverless Architecture but on the other hand there are a Drawbacks.

## AWS Amplify

### How it works

AWS Amplify is a set of purpose-built tools and services that makes it quick and easy for front-end web and mobile developers build full-stack applications on AWS.

## API (GRAPHQL)

* The GraphQL allows us to quickly create backends for your web and mobile applications on AWS. With the GraphQL Transform

* The GraphQL Transform simplifies the process of developing, deploying, and maintaining GraphQL APIs.

### Create a GraphQL API

1. In the root of project run `amplify init`.
2. Follow the wizard to create a new app. After finishing the wizard run `amplify add api` then Select the following options:

    * Select GraphQL
    * When asked if you have a schema, say No
    * Select one of the default samples; you can change this later
    * Choose to edit the schema and it will open the new schema.graphql in your editor

3. run `amplify push`.

### Test the API

To test the API you can run `amplify mock api`.

### Update schema

1. open your project's backend/api/~apiname~/schema.graphql file (NOT the one in the backend/api/~apiname~/build folder) and edit it.

2. Compile the backend/api/~apiname~/schema.graphql by running `amplify api gql-compile`

3. Push updated changes with `amplify push`

### Rebuild GraphQL API

Rebuild should NEVER be used in a production environment! and to rebuild the API you can run `amplify rebuild api`

### API Category Project Structure

API directory will have the following:

1. build/
2. resolvers/
3. stacks/
4. parameters.json
5. schema.graphql
6. schema/
7. transform.conf.json

## Resources used in this reading

1. [What is Serverless Architecture](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)
2. [AWS Amplify](https://aws.amazon.com/ar/amplify/)
3. [API (GRAPHQL)](https://docs.amplify.aws/cli/graphql-transformer/overview/)