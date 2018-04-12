## v6.0.0 (2018-04-12):

### NEW FEATURES


* [`a9e722118`](https://github.com/npm/npm/commit/a9e7221181dc88e14820d0677acccf0648ac3c5a)
  [#20256](https://github.com/npm/npm/pull/20256)
  add support for managing npm hooks
  ([@zkat](https://github.com/zkat))

* [`cf4d7b4de`](https://github.com/npm/npm/commit/cf4d7b4de6fa241a656e58f662af0f8d7cd57d21)
  [#20257](https://github.com/npm/npm/pull/20257)
  add shasum and integrity info to preview
  ([@zkat](https://github.com/zkat))
* [`8a1a64203`](https://github.com/npm/npm/commit/8a1a64203cca3f30999ea9e160eb63662478dcee)
  [#20126](https://github.com/npm/npm/pull/20126)
  add npm cit command
  ([@SimenB](https://github.com/SimenB))

* [`fe867aaf1`](https://github.com/npm/npm/commit/fe867aaf19e924322fe58ed0cf0a570297a96559)
  Stop churning ranges back to versions in requires
  ([@iarna](https://github.com/iarna))
* [`49d18b4d8`](https://github.com/npm/npm/commit/49d18b4d87d8050024f8c5d7a0f61fc2514917b1)
  Upgrade all requires to ranges
  ([@iarna](https://github.com/iarna))
* [`ff6b31f77`](https://github.com/npm/npm/commit/ff6b31f775f532bb8748e8ef85911ffb35a8c646)
  Update npm's lockfile to ranges from versions
  ([@iarna](https://github.com/iarna))
* [`78eab3cda`](https://github.com/npm/npm/commit/78eab3cdab6876728798f876d569badfc74ce68f)
  Upgrade package-lock
  ([@iarna](https://github.com/iarna))

### BUG FIXES

* [`685764308`](https://github.com/npm/npm/commit/685764308e05ff0ddb9943b22ca77b3a56d5c026)
  treat otps as strings to not eat leading zeros
  ([@iarna](https://github.com/iarna))

* [`8f3faa323`](https://github.com/npm/npm/commit/8f3faa3234b2d2fcd2cb05712a80c3e4133c8f45)
  Allow through bundled deps w/o modern meta
  ([@iarna](https://github.com/iarna))
* [`6800f76ff`](https://github.com/npm/npm/commit/6800f76ffcd674742ba8944f11f6b0aa55f4b612)
  Remove needless asynchrony
  ([@iarna](https://github.com/iarna))
* [`ec90c06c7`](https://github.com/npm/npm/commit/ec90c06c78134eb2618612ac72288054825ea941)
  Make duplicate actions impossible
  ([@iarna](https://github.com/iarna))
* [`825b5d2c6`](https://github.com/npm/npm/commit/825b5d2c60e620da5459d9dc13d4f911294a7ec2)
  Ensure sources for bundled modules exist
  ([@iarna](https://github.com/iarna))
* [`4785f13fb`](https://github.com/npm/npm/commit/4785f13fb69f33a8c624ecc8a2be5c5d0d7c94fc)
  Ensure all actions survive the sort
  ([@iarna](https://github.com/iarna))
* [`bd16485f5`](https://github.com/npm/npm/commit/bd16485f5b3087625e13773f7251d66547d6807d)
  Only avoid adding bundled deps when they're the result of a link
  ([@iarna](https://github.com/iarna))

* [`429498a8c`](https://github.com/npm/npm/commit/429498a8c8d4414bf242be6a3f3a08f9a2adcdf9)
  [#20029](https://github.com/npm/npm/pull/20029)
  allow fakeChildren for non-integrity types
  ([@zkat](https://github.com/zkat))

* [`834b46ff4`](https://github.com/npm/npm/commit/834b46ff48ade4ab4e557566c10e83199d8778c6)
  [#20122](https://github.com/npm/npm/pull/20122)
  shinier update-notifier
  This message is based on the one pnpm uses, which
  I think takes care of all the false update messages and
  missing -g that happens with the default notifier message.
  It also tells people what "level" the update is.
  ([@zkat](https://github.com/zkat))

* [`f9de7ef3a`](https://github.com/npm/npm/commit/f9de7ef3a1089ceb2610cd27bbd4b4bc2979c4de)
  [#20154](https://github.com/npm/npm/pull/20154)
  Let version succeed when `package-lock.json` is gitignored
  ([@nwoltman](https://github.com/nwoltman))

* [`f8ec52073`](https://github.com/npm/npm/commit/f8ec520732bda687bc58d9da0873dadb2d65ca96)
  [#20212](https://github.com/npm/npm/pull/20212)
  only create config dir before write
  This change fixes the bug that creates
  unnecessary ./etc folder when calling npm
  with the --prefix flag.
  ([@buddydvd](https://github.com/buddydvd))

* [`ab489b753`](https://github.com/npm/npm/commit/ab489b75362348f412c002cf795a31dea6420ef0)
  [#20140](https://github.com/npm/npm/pull/20140)
  note that package-lock version gets touched by npm-version
  ([@srl295](https://github.com/srl295))

* [`857c2138d`](https://github.com/npm/npm/commit/857c2138dae768ea9798782baa916b1840ab13e8)
  [#20032](https://github.com/npm/npm/pull/20032)
  Fix messaging for 401 errors that lack a reason
  Prevously they were falling through to 404 handling and being printed as:
  npm ERR! 404 Registry returned 401 for DELETE on …
  ([@iarna](https://github.com/iarna))

* [`d2d290bca`](https://github.com/npm/npm/commit/d2d290bcaa85e44a4b08cc40cb4791dd4f81dfc4)
  [#20082](https://github.com/npm/npm/pull/20082)
  allow optional @ prefix on scope
  ([@bcoe](https://github.com/bcoe))

* [`b5babf0a9`](https://github.com/npm/npm/commit/b5babf0a9aa1e47fad8a07cc83245bd510842047)
  [#19580](https://github.com/npm/npm/pull/19580)
  Better message when an "OTP" error occurs
  ([@jdeniau](https://github.com/jdeniau))

* [`471ee1c5b`](https://github.com/npm/npm/commit/471ee1c5b58631fe2e936e32480f3f5ed6438536)
  install/deps: fix bug where optional status not saved to package-lock
  Specifically, because we weren't adding optional deps to both `dependencies`
  and `optionalDependencies` (the way `normalize-package-data` does), it meant
  that `computeMetadata` didn't think the dep was actually required and as such
  there was no way to compute its optional status.
  ([@iarna](https://github.com/iarna))
* [`b3f98d8ba`](https://github.com/npm/npm/commit/b3f98d8ba242a7238f0f9a90ceea840b7b7070af)
  Filter optional deps during diff-trees
  This allows `--no-optional` runs to include optional dependencies in the
  lockfile while excluding them from installation on disk.
  ([@iarna](https://github.com/iarna))
* [`9dea95e31`](https://github.com/npm/npm/commit/9dea95e319169647bea967e732ae4c8212608f53)
  Read optional status from shrinkwrap when we have to
  ([@iarna](https://github.com/iarna))
* [`3888d2051`](https://github.com/npm/npm/commit/3888d20517593095038caa3cff68d697ae8769a8)
  Synthetic link deps get the right realpath
  ([@iarna](https://github.com/iarna))
* [`0da38b7b4`](https://github.com/npm/npm/commit/0da38b7b4aff0464c60ad12e0253fd389efd5086)
  Ensure optional status is saved to lock file
  ([@iarna](https://github.com/iarna))

### MISCELLANEOUS

* [`ec6b12099`](https://github.com/npm/npm/commit/ec6b120995c9c1d17ff84bf0217ba5741365af2d)
  Exclude all tests from the published version of npm itself.
  ([@iarna](https://github.com/iarna))

### DEPENDENCY UPDATES

* [`73dc97455`](https://github.com/npm/npm/commit/73dc974555217207fb384e39d049da19be2f79ba)
  [zkat/cipm#46](https://github.com/zkat/cipm/pull/46)
  `libcipm@1.6.2`:
  Detect binding.gyp for default install lifecycle. Let's `npm ci` work on projects that
  have their own C code.
  ([@caleblloyd](https://github.com/caleblloyd))
* [`77c3f7a00`](https://github.com/npm/npm/commit/77c3f7a0091f689661f61182cd361465e2d695d5)
  `iferr@1.0.0`
* [`dce733e37`](https://github.com/npm/npm/commit/dce733e37687c21cb1a658f06197c609ac39c793)
  [zkat/json-parse-better-errors#1](https://github.com/zkat/json-parse-better-errors/pull/1)
  `json-parse-better-errors@1.0.2`
  ([@Hoishin](https://github.com/Hoishin))
* [`c52765ff3`](https://github.com/npm/npm/commit/c52765ff32d195842133baf146d647760eb8d0cd)
  `readable-stream@2.3.6`
  ([@mcollina](https://github.com/mcollina))
* [`e160adf9f`](https://github.com/npm/npm/commit/e160adf9fce09f226f66e0892cc3fa45f254b5e8)
  `update-notifier@2.4.0`
  ([@sindersorhus](https://github.com/sindersorhus))
* [`9a9d7809e`](https://github.com/npm/npm/commit/9a9d7809e30d1add21b760804be4a829e3c7e39e)
  `marked@0.3.1`
  ([@joshbruce](https://github.com/joshbruce))
* [`f2fbd8577`](https://github.com/npm/npm/commit/f2fbd857797cf5c12a68a6fb0ff0609d373198b3)
  [#20256](https://github.com/npm/npm/pull/20256)
  `figgy-pudding@2.0.1`
  ([@zkat](https://github.com/zkat))
* [`44972d53d`](https://github.com/npm/npm/commit/44972d53df2e0f0cc22d527ac88045066205dbbf)
  [#20256](https://github.com/npm/npm/pull/20256)
  `libnpmhook@3.0.0`
  ([@zkat](https://github.com/zkat))
* [`cfe562c58`](https://github.com/npm/npm/commit/cfe562c5803db08a8d88957828a2cd1cc51a8dd5)
  [#20276](https://github.com/npm/npm/pull/20276)
  `node-gyp@3.6.2`
* [`3c0bbcb8e`](https://github.com/npm/npm/commit/3c0bbcb8e5440a3b90fabcce85d7a1d31e2ecbe7)
  [zkat/npx#172](https://github.com/zkat/npx/pull/172)
  `libnpx@10.1.1`
  ([@jdalton](https://github.com/jdalton))
* [`0573d91e5`](https://github.com/npm/npm/commit/0573d91e57c068635a3ad4187b9792afd7b5e22f)
  [zkat/cacache#128](https://github.com/zkat/cacache/pull/128)
  `cacache@11.0.1`
  ([@zkat](https://github.com/zkat))
* [`396afa99f`](https://github.com/npm/npm/commit/396afa99f61561424866d5c8dd7aedd6f91d611a)
  `figgy-pudding@3.1.0`
  ([@zkat](https://github.com/zkat))
* [`e7f869c36`](https://github.com/npm/npm/commit/e7f869c36ec1dacb630e5ab749eb3bb466193f01)
  `pacote@8.0.0`
  ([@zkat](https://github.com/zkat))
* [`77dac72df`](https://github.com/npm/npm/commit/77dac72dfdb6add66ec859a949b1d2d788a379b7)
  `ssri@6.0.0`
  ([@zkat](https://github.com/zkat))
* [`0b802f2a0`](https://github.com/npm/npm/commit/0b802f2a0bfa15c6af8074ebf9347f07bccdbcc7)
  `retry@0.12.0`
  ([@iarna](https://github.com/iarna))
* [`4781b64bc`](https://github.com/npm/npm/commit/4781b64bcc47d4e7fb7025fd6517cde044f6b5e1)
  `libnpmhook@4.0.1`
  ([@zkat](https://github.com/zkat))
* [`7bdbaeea6`](https://github.com/npm/npm/commit/7bdbaeea61853280f00c8443a3b2d6e6b893ada9)
  `npm-package-arg@6.1.0`
  ([@zkat](https://github.com/zkat))
* [`5f2bf4222`](https://github.com/npm/npm/commit/5f2bf4222004117eb38c44ace961bd15a779fd66)
  `read-package-tree@5.2.1`
  ([@zkat](https://github.com/zkat))

## v6.0.0-0 (2018-03-23):

Sometimes major releases are a big splash, sometimes they're something
smaller.  This is the latter kind.  That said, we expect to keep this in
release candidate status until Node 10 ships at the end of April.  There
will likely be a few more features for the 6.0.0 release line between now
and then.  We do expect to have a bigger one later this year though, so keep
an eye out for `npm@7`!

### *BREAKING* AVOID DEPRECATED

When selecting versions to install, we now avoid deprecated versions if
possible. For example:

```
Module: example
Versions:
1.0.0
1.1.0
1.1.2
1.1.3 (deprecated)
1.2.0 (latest)
```

If you ask `npm` to install `example@~1.1.0`, `npm` will now give you `1.1.2`.

By contrast, if you installed `example@~1.1.3` then you'd get `1.1.3`, as
it's the only version that can match the range.

* [`78bebc0ce`](https://github.com/npm/npm/commit/78bebc0cedc4ce75c974c47b61791e6ca1ccfd7e)
  [#20151](https://github.com/npm/npm/pull/20151)
  Skip deprecated versions when possible.
  ([@zkat](https://github.com/zkat))

### *BREAKING* UPDATE AND OUTDATED

When `npm install` is finding a version to install, it first checks to see
if the specifier you requested matches the `latest` tag.  If it doesn't,
then it looks for the highest version that does.  This means you can do
release candidates on tags other than `latest` and users won't see them
unless they ask for them.  Promoting them is as easy as setting the `latest`
tag to point at them.

Historically `npm update` and `npm outdated` worked differently.  They just
looked for the most recent thing that matched the semver range, disregarding
the `latest` tag. We're changing it to match `npm install`'s behavior.

* [`3aaa6ef42`](https://github.com/npm/npm/commit/3aaa6ef427b7a34ebc49cd656e188b5befc22bae)
  Make update and outdated respect latest interaction with semver as install does.
  ([@iarna](https://github.com/iarna))
* [`e5fbbd2c9`](https://github.com/npm/npm/commit/e5fbbd2c999ab9c7ec15b30d8b4eb596d614c715)
  `npm-pick-manifest@2.1.0`
  ([@iarna](https://github.com/iarna))

### PLUS ONE SMALLER PATCH

Technically this is a bug fix, but the change in behavior is enough of an
edge case that I held off on bringing it in until a major version.

When we extract a binary and it starts with a shebang (or "hash bang"), that
is, something like:

```
#!/usr/bin/env node
```

If the file has Windows line endings we strip them off of the first line. 
The reason for this is that shebangs are only used in Unix-like environments
and the files with them can't be run if the shebang has a Windows line ending.

Previously we converted ALL line endings from Windows to Unix.  With this
patch we only convert the line with the shebang.  (Node.js works just fine
with either set of line endings.)

* [`814658371`](https://github.com/npm/npm/commit/814658371bc7b820b23bc138e2b90499d5dda7b1)
  [`7265198eb`](https://github.com/npm/npm/commit/7265198ebb32d35937f4ff484b0167870725b054)
  `bin-links@1.1.2`:
  Only rewrite the CR after a shebang (if any) when fixing up CR/LFs.
  ([@iarna](https://github.com/iarna))

### *BREAKING* SUPPORTED NODE VERSIONS

Per our supported Node.js policy, we're dropping support for both Node 4 and
Node 7, which are no longer supported by the Node.js project.

* [`077cbe917`](https://github.com/npm/npm/commit/077cbe917930ed9a0c066e10934d540e1edb6245)
  Drop support for Node 4 and Node 7.
  ([@iarna](https://github.com/iarna))

### DEPENDENCIES

* [`478fbe2d0`](https://github.com/npm/npm/commit/478fbe2d0bce1534b1867e0b80310863cfacc01a)
  `iferr@1.0.0`
* [`b18d88178`](https://github.com/npm/npm/commit/b18d88178a4cf333afd896245a7850f2f5fb740b)
  `query-string@6.0.0`
* [`e02fa7497`](https://github.com/npm/npm/commit/e02fa7497f89623dc155debd0143aa54994ace74)
  `is-cidr@2.0.5`
* [`c8f8564be`](https://github.com/npm/npm/commit/c8f8564be6f644e202fccd9e3de01d64f346d870)
  [`311e55512`](https://github.com/npm/npm/commit/311e5551243d67bf9f0d168322378061339ecff8)
  `standard@11.0.1`
