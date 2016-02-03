# Thumbor Scalingo

This is a quick start project for setting up a Thumbor instance on Scalingo.

## Getting started (One-Click Deployment)

[![Deploy to Scalingo](https://cdn.scalingo.com/deploy/button.svg)](https://my.scalingo.com/deploy)

Deploying Thumbor on Scalingo is as easy as clicking on **Deploy to Scalingo** button and giving it a name.

On the deployment page, you can optionally change `ALLOW_UNSAFE_URL` to `False` and use the generated `SECURITY_KEY` in your client apps.

## Accessing your Thumbor

Once deployed, you can open your browser and go to your Thumbor, e.g. `my-thumbor.scalingo.io/unsafe/0x0/https://avatars.githubusercontent.com/u/4868969`.

Notice the **unsafe** path in the URL, this URL only works with `ALLOW_UNSAFE_URL` set to `True`.

## Customizing you Thumbor

The deployed instance is a working Thumbor that can be used as is, but you may want to customize it and change the security policy. For further details, please refer to [Thumbor documentation](https://github.com/thumbor/thumbor/wiki).

To retrieve the deployed project, you can use the command:

```bash
git clone git@scalingo.com:my-thumbor.git
```

You can then make changes to the project (e.g. adding storage) and deploy the update by doing:

```bash
git push scalingo master
```
