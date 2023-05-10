# A Minimalistic Photography Portfolio website using Next.js 13 and DatoCMS

This example showcases a TypeScript Next.js 13 website with App Router (app) — using [DatoCMS](https://www.datocms.com/) as the data source.

It uses the awesome [@graphql-codegen/client-preset](https://the-guild.dev/graphql/codegen/plugins/presets/preset-client) package to offer typed GraphQL queries.

The purpose of this repo is to have a quick start reference that can be set up with the "one-click" button below.

## Demo

Have a look at the end result live:

### [https://datocms-minimalistic-photography-website.vercel.app/](https://datocms-minimalistic-photography-website.vercel.app/)

## How to use

### Quick start

1. [Create an account on DatoCMS](https://datocms.com).

2. Make sure that you have set up the [Github integration on Vercel](https://vercel.com/docs/git/vercel-for-github).

3. Let DatoCMS set everything up for you clicking this button below:

[![Deploy with DatoCMS](https://dashboard.datocms.com/deploy/button.svg)](https://dashboard.datocms.com/deploy?repo=datocms/next-minimalistic-photography:main)

:warning: Remember to setup FormSpark (see step below), as it's needed for the contact form to work!

### Setup FormSpark

1. Signup to https://formspark.io/
2. Create a new form - the first 250 form submissions are free!
3. Go to Settings, and [copy the Form ID](https://github.com/datocms/next-minimalistic-photography/blob/main/docs/minimalistic-photography.png)
4. Paste the same ID in your DatoCMS project, under the "Contact Page" > "FormSpark Form ID" field.

### Local setup

Once the setup of the project and repo is done, clone the repo locally.

#### Set up environment variables

In your DatoCMS' project, go to the **Settings** menu at the top and click **API tokens**.

Then click **Read-only API token** and copy the token.

Next, copy the `.env.example` file in this directory to `.env` (which will be ignored by Git):

```bash
cp .env.local.sample .env.local
```

and set the `NEXT_DATOCMS_API_TOKEN` variable as the API token you just copied.

#### Run your project locally

```bash
npm install
npm run dev
```

Your blog should be up and running on [http://localhost:3000](http://localhost:3000)!

## VS Code

It's strongly suggested to install the [GraphQL: Language Feature Support](https://marketplace.visualstudio.com/items?itemName=GraphQL.vscode-graphql) extension, to get autocomplete suggestions, validation against schema, and many more niceties when working with your GraphQL queries.

