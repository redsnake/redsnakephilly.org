## Redsnake Philly

The RedSnake is an annual event where Rubyists and Pythonistas get together to throw down some hard tech and inspire each other to level up. Ultimately we aim to accomplish the following:

- To be the premier technical event for hardcore programmers in Philadelphia
- To inspire and provide an environment of learning to those who are new to programming
- To introduce Philadelphia's top companies to Philadelphia's top programmers
- To raise national recognition for Philadelphia&#8217;s tech community and attract top talent to the city

The format is 2 hours of alternating 10 minute lightning talks. It's intense, technical, and mind blowing.


## What's this?

This is the Octopress site for redsnakephilly.org, published via Github pages.

## How do I update the site?

To hack on this site:
- Clone this repo: `git clone git@github.com:redsnake/redsnakephilly.org.git`

I like to use RVM to make a sanitary build environment. The following should set up Ruby in an RVM and install the appropriate gems you need to work:

```bash
cd redsnakephilly.org
rvm gemset create redsnakephilly
rvm use redsnakephilly
rvm install

```

Make updates in the `source/` directory. Use `rake preview` to see the changes. Use `rake generate && rake deploy` to commit the changes to the `gh-pages` branch and push them to Github.
