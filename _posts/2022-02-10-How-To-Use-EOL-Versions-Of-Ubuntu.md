---
published: true
---
Canonical makes most of their money selling ESM, so that businesses can continue to use EOL versions of Ubuntu for servers. That's no secret. But, what many people don't know, is that you can grab a free token so that you can use Extended Support Maintenance for personal use. It allows you to run Ubuntu 16.04 and even 14.04 for an extended period of time, while still getting security updates. So, if you would like to use an older version of Ubuntu while not having to worry about having your security compromised, I am going to show you how to get your token, install the Ubuntu Advantage Tools, and attach your token.

# Getting Your Token

For personal use, you can go to this link. Here you will have to use your email to register for an Ubuntu One account. Then, you can simply follow the instructions to get your free token.

[Click Me!](https://ubuntu.com/advantage)

# Installing Ubuntu Advantage Tools 

Before you can use ESM, you will have to install Ubuntu tools to use your token. On Ubuntu, you can just use this command.

        sudo apt install ubuntu-advantage-tools

This will give you the UA client, which you will need for the next step.

# Enabling ESM With Your Token

Using the UA client, you can use your token to enable ESM like so.

        sudo ua attach INSERT_TOKEN_HERE

When attaching your token, ESM will automatically be enabled. If you would like to check if it is really enabled, you can type this to see that it is in fact enabled.

        sudo ua status

# You're Done! 

Now, you can enjoy 14.04 and 16.04 for another 3 and 5 years respectively while still getting security updates. Whether you need an old version of Ubuntu for your server, or you just would like to have a super stable desktop, Ubuntu ESM is a great option for you. Give it a try, you'll be surprised how good old versions of Ubuntu are.
~                                                                                                                                                                                           
~
