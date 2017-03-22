# Symphony Extensions Network

##### The central place to discuss, organize and optimize the Symphony CMS extensions ecosystem.

**Note:** _Besides serving as an issue tracker for symphonyextensions.com and all things related to the extensions ecosystem this repository aims to provide a comprehensive set of best practices, guidelines and resources regarding extension development and maintenance. We encourage every extension developer to not only keep an eye on this repository (watch/star), but to join the discussion and help us build a platform that in the long run finally might define who, what and wherefore the "symphonists" are :)_

<br/>

## Scope & Focus

1. [ ] 1. Extension Ecosystem
2. [ ] 2. Extension Development
3. [x] 3. **[Extension Publishing](#3-extension-publishing)**
4. [ ] 4. Extension Migration
5. [x] 5. **[Extension Adoption](#5-extension-adoption)**
6. [ ] 6. Extension Transfer
7. [ ] 7. Extension Consolidation
8. [ ] 8. Extension Deprecation
9. [ ] 9. Extension Request

<br/>

## 3. Extension Publishing

If you built an extension that might also be useful for other Symphony developers you should think about publishing it. Here's a list of **best practices** you should follow if you want to share your work with the community:

### A) Branches, Releases & Version Numbers

1. Use **[branches](https://guides.github.com/introduction/flow/)** to develop and maintain your extension on github. Your basic setup should contain a `master`-branch (representing the latest stable, tested and documented release) and an `integration`-branch (that is used for ongoing development and incoming pull requests and should cointain stable code too). Experimental and instable stuff should happen in separate feature-branches.
2. Use **[releases](https://help.github.com/articles/creating-releases/)** to publish versions of your extension on github.
3. Use **[semantic versioning](http://semver.org/)** for your extension's version numbers. 
4. Use **[tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging)** to tag you releases with the appropriate version number. Don't follow github's recommendation of adding a prefixed `v`, just use the plain version numbers as tag (e.g. `1.0.0` instead of `v1.0.0`)
5. Add a short **changelog** to each release listing all relevant changes since the previous release.

### B) Metadata, Documentation & Licenses

1. Get familiar with the official **[Symphony Extension Metadata Schema](http://symphonyextensions.com/schemas/extension/1.0/)** and add a valid and comprehensive **[extension.meta.xml](http://symphonyextensions.com/schemas/extension/1.0/#example)** to your repo.
2. Add a descriptive **[markdown](https://guides.github.com/features/mastering-markdown/)**-formatted **[readme](https://help.github.com/articles/about-readmes/)** to your repo explaining what your extension does and how to use it.
3. Keep your **readme** focussed. You don't have to include _everything_ in here – **[github wikis](https://help.github.com/articles/about-github-wikis/)** are a great way of providing additional documentation, tutorials or examples. <sup><a href="#extension-publishing-f1">1</a></sup>
4. _If_ you set up a **wiki** you should mention it in the **readme**. A list of links to all wiki pages ain't a bad idea either.
5. Make use of **[github topics](https://help.github.com/articles/about-topics/)** to tag your repo: [`symphony-cms`](https://github.com/search?q=topic%3Asymphony-cms) and [`symphony-cms-extension`](https://github.com/search?q=topic%3Asymphony-cms-extension) are the official recommended tags for each extension-repository. Depending on the scope of your extension you might also want to add more specific topics (following the `symphony-cms-xyz`-syntax, e.g. [`symphony-cms-multilingual`](https://github.com/search?q=topic%3Asymphony-cms-multilingual)).
6. Add a valid **[licence](https://help.github.com/articles/licensing-a-repository/)** to your repo – **[MIT](https://choosealicense.com/licenses/mit/)** is a good choice that's used by Symphony itself too.


### C) Publishing Platforms

1. Publish your extension on **[github](https://github.com/)**
2. Publish your extension on **[symphonyextensions.com](http://symphonyextensions.com/)**
3. You might also want to spread the word in the official **[chat](https://gitter.im/symphonycms/symphony-2)** or **[forums](http://www.getsymphony.com/discuss/)** to get some feedback about your extension.
4. The official **[Symphony website](http://www.getsymphony.com/download/extensions/)** also houses a collection of extensions but we don't recommend publishing new extensions there at the moment.

<br/>
<p>
	<sup>
		<b id="extension-publishing-f1">1)</b> This holds especially true if you plan to include <b>tables</b> in your readme – they're <a href="https://github.com/symphonists/symphony-extensions-network/issues/5">not supported</a> on <a href="http://symphonyextensions.com/">symphonyextensions.com</a> and are better of in a wiki.  
	</sup>
</p>
<br/>


## 5. Extension Adoption

If you own extensions that you no longer want to support, update or care about we'd encourage you to take the following steps to help us find a new home for them:

1. Submit a [new issue](https://github.com/symphonists/symphony-extensions-network/issues/new) (one per extension).
2. Give it a descriptive title: _"Extension Adoption: Extension Name"_.
3. Add a link to the extension repository.
4. Optionally add a short statement about the current state of the extension.
5. If possible give Nicolas ([@nitriques](https://github.com/nitriques)) admin access to the repo so he can manage the transfer for you. <sup><a href="#extension-adoption-f1">1</a></sup>

Depending on the state, popularity and usefulness of the extension we will then either …

- … try to find a developer who is willing to take over ownership and further maintenance/development.
- … transfer the repo to the symphonists organization and provide best possible support there.
- … mark the extension as deprecated and transfer it to the "symphonists archives".

If you don't give Nicolas admin access to the repo we'll need you to take action after a solution is agreed upon. Thus it would be great if you could keep an eye on the discussion and be available to manage the [repo transfer](https://help.github.com/articles/transferring-a-repository/) yourself.

<br/>
<p>
	<sup>
		<b id="extension-adoption-f1">1)</b> If the repository is owned by a user account you might need to set up a temporary organization to give other users permission to transfer the repository.  Please refer to the github help for details about <a href="https://help.github.com/articles/transferring-a-repository/">transferring a repository</a> and <a href="https://help.github.com/articles/repository-permission-levels-for-an-organization/">repository permission levels</a>. 
	</sup>
</p>
<br/>
