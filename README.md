# ihatemarkdown
Nothing to see here. Just a place to try markdown on my README so I don't fuck up other projects READMES.

## Contributing

To add code to go4, send a pull request or push a change to Gerrithub.

We assume you already have your $GOPATH set and the go4 code cloned at
$GOPATH/src/go4.org. For example:

* `git clone https://review.gerrithub.io/camlistore/go4 $GOPATH/src/go4.org`

### To push a code review to Gerrithub directly:

* Sign in to [http://gerrithub.io](http://gerrithub.io "Gerrithub") with your Github account.

* Install the git hook that adds the magic "Change-Id" line to your commit messages:

`curl -o $GOPATH/src/go4.org/.git/hooks/commit-msg https://camlistore.googlesource.com/camlistore/+/master/misc/commit-msg.githook`

* make changes

* commit (the unit of code review is a single commit identified by the Change-ID, **NOT** a series of commits on a branch)

* `git push ssh://$YOUR_GITHUB_USERNAME@review.gerrithub.io:29418/camlistore/go4 HEAD:refs/for/master`

### Using Github Pull Requests

* send a pull request with a single commit

* create a Gerrithub code review at https://review.gerrithub.io/plugins/github-plugin/static/pullrequests.html, selecting the pull request you just created.

### Problems contributing?

* Please file an issue or contact the [Camlistore mailing list](https://groups.google.com/forum/#!forum/camlistore) for any problems with the above.

See [https://review.gerrithub.io/Documentation/user-upload.html](https://review.gerrithub.io/Documentation/user-upload.html) for more generic documentation.

(TODO: more docs on Gerrit, integrate git-codereview, etc.)

curl -o $GOPATH/src/go4.org/.git/hooks/commit-msg https://camlistore.googlesource.com/camlistore/+/master/misc/commit-msg.githook

curl -o $GOPATH/src/go4.org/.git/hooks/commit-msg https://camlistore.googlesource.com/camlistore/+/master/misc/commit-msg.githook