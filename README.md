# ihatemarkdown
Nothing to see here. Just a place to try markdown on my README so I don't fuck up other projects READMES.

## Contributing

To add code to go4, send a pull request or push a change to Gerrithub.

We assume you already have your $GOPATH set and the go4 code cloned at
$GOPATH/src/go4.org. For example:

<ul>
<li><code>git clone https://review.gerrithub.io/camlistore/go4 $GOPATH/src/go4.org</code></li>
</ul>

### To push a code review to Gerrithub directly:

<ul>
<li><p>Sign in to <a href="http://gerrithub.io" title="Gerrithub">http://gerrithub.io</a> with your Github account.</p></li>
<li><p>Install the git hook that adds the magic "Change-Id" line to your commit messages:</p>
<p><code>curl -o $GOPATH/src/go4.org/.git/hooks/commit-msg https://camlistore.googlesource.com/camlistore/+/master/misc/commit-msg.githook</code></p></li>
<li><p>make changes</p></li>
<li><p>commit (the unit of code review is a single commit identified by the Change-ID, <strong>NOT</strong> a series of commits on a branch)</p></li>
<li><p><code>git push ssh://$YOUR<em>GITHUB</em>USERNAME@review.gerrithub.io:29418/camlistore/go4 HEAD:refs/for/master</code></p></li>
</ul>

### Using Github Pull Requests

* send a pull request with a single commit

* create a Gerrithub code review at https://review.gerrithub.io/plugins/github-plugin/static/pullrequests.html, selecting the pull request you just created.

### Problems contributing?

* Please file an issue or contact the [Camlistore mailing list](https://groups.google.com/forum/#!forum/camlistore) for any problems with the above.

See [https://review.gerrithub.io/Documentation/user-upload.html](https://review.gerrithub.io/Documentation/user-upload.html) for more generic documentation.

(TODO: more docs on Gerrit, integrate git-codereview, etc.)

