# Welcome to Remix!

- [Remix Docs](https://remix.run/docs)
- [Architect Docs](https://arc.codes)

## Architect Setup

When deploying to AWS Lambda with Architect, you'll need the AWS SDK.

Architect recommends installing `aws-sdk` globally:

```sh
$ npm install --global aws-sdk
```

## Development

```
npm install # in case you haven't already
```

You will be running two processes during development when using Architect as your server.

- Your Architect Sandbox server to emulate AWS
- The Remix watch process to build your Remix app

```sh
# these can be run simultaneously with:
$ npm run dev
```

* You may need to exit this command twice (ctrl + c) to end both processes.

Open up [http://localhost:3333](http://localhost:3333) and you should be ready to go!

## Deploying

Before you can deploy, you'll need to do some setup with AWS:

- First [install the AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- Then [follow the Architect setup instructions](https://arc.codes/docs/en/guides/get-started/detailed-aws-setup).

If you make it through all of that, you're ready to deploy!

1. build the app for production:

   ```sh
   $ npm run build
   ```

2. Deploy with `arc`

   ```sh
   $ npx arc deploy production
   ```

You're in business!
