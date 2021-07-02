# Real world Ruby apps

> Real World Ruby apps and their open source codebases for developers to learn from

You'll find the source code in the [`apps/`](apps/) subdirectory. These apps
are:

- Executable via the command line
- Not based on any framework (see [other
  repos](#other-real-world-codebase-collections) for Rails, Sinatra, etc.)

Thank you to every developer who has worked on a project this repo links to,
your work is helping developers learn Ruby.

## How to install on your computer

```bash
# Clone this git repo:
git clone git@github.com:jeromedalbert/real-world-ruby-apps.git

cd real-world-ruby-apps/

# The apps are linked to as git submodules.
# This will take some time... (see comment below for possible speedup)
git submodule update --init

# OR if you've got git 2.9+ installed try to run updates in parallel:
# git submodule update --init --jobs 4
```

## Other Real World codebase collections

- Real World Rails https://github.com/eliotsykes/real-world-rails
- Real World Sinatra https://github.com/jeromedalbert/real-world-sinatra
- Real World Ember https://github.com/eliotsykes/real-world-ember
- Real World React Apps https://github.com/jeromedalbert/real-world-react-apps
- Know any others? Please open a PR and add the link here

## Information for contributors

#### Is your app the right fit?

- The majority of the codebase should not be based on any framework, like Rails
  or Sinatra. There are dedicated Real World repos for these.
- The vast majority of the codebase should be written in Ruby.
- The main app should be executable via a binary.
- The app should be somewhat popular, in order to limit the apps in this repo
  to a manageable amount. There is some leeway in what constitutes a popular
  app. A possible indicator can be GitHub stars compared to similar apps.

Don't hesitate to submit a pull request if you meet the criteria!

#### How to add a Real World app

Given a GitHub repo for an app `githubuser/foo`:

```bash
# Inside the project root:
git submodule add -b master git@github.com:githubuser/foo.git apps/foo
```

#### Updating the apps submodules to latest

The apps in `apps/` are git submodules. Git submodules are locked to a revision
and don't stay in sync with the latest revision.

To update the revisions, run:

```bash
# This will take some time:
git submodule foreach git pull origin master
```

---

# Contributors

- Jerome Dalbert http://jeromedalbert.com
- Contributions are welcome, fork the GitHub repo, make your changes, then
  submit your pull request! Reach out if you'd like some help.
