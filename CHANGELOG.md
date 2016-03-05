<<<<<<< HEAD
# Python Buildpack Changelog

## v70 (2015-10-29)

Improved compatibility with multi and node.js buildpacks.

## v69 (2015-10-12)

Revert to v66.

## v68 (2015-10-12)

Fixed .heroku/venv error with modern apps.

## v67 (2015-10-12)

Further improved cache compatibility with multi and node.js buildpacks.

## v66 (2015-10-09)

Improved compatibility with multi and node.js buildpacks.

## v65 (2015-10-08)

Reverted v64.

## v64 (2015-10-08)

Improved compatibility with multi and node.js buildpacks.

## v63 (2015-10-08)

Updated Pip and Setuptools.

- Setuptools updated to v18.3.2
- Pip updated to v7.1.2


## v62 (2015-08-07)

Updated Pip and Setuptools.

- Setuptools updated to v18.1
- Pip updated to v7.1.0

## v61 (2015-06-30)

Updated Pip and Setuptools.

- Setuptools updated to v18.0.1
- Pip updated to v7.0.3

## v60 (2015-05-27)

Default Python is now latest 2.7.10. Updated Pip and Distribute.

- Default Python version is v2.7.10
- Setuptools updated to v16.0
- Pip updated to v7.0.1
=======
# Node.js Buildpack Changelog

## v88 (2016-2-23)

- Retries all curl requests
- Use HTTPS for node binary downloads again

## v87 (2015-11-03)

Several edge-case fixes

- Enables compiling the same directory multiple times
- Updates tests for Node v5
- Moves node_modules/.bin binaries to last on the PATH

## v86 (2015-10-08)

Fixes piped output buffering issues

## v85 (2015-10-08)

Fixes piped output buffering issues (unsuccessful)

- https://github.com/heroku/heroku-buildpack-nodejs/issues/273

## v84 (2015-10-08)

Replaces sed with awk for output formatting

- large output (from assets or npm 3) was crashing sed ('resource unavailable')

## v83 (2015-10-05)

Caching improvements

- Fixes modules-checked-in reference URL
- When cache restoration is disabled, empties the cache instead of saving it
- Adds bower_components as a default cache target

## v82 (2015-09-30)

Detects bower+angular resolution failures
Detects missing grunt/gulp/bower failures

## v81 (2015-09-24)

Supports WEB_CONCURRENCY=28 for Performance-L dynos

## v80 (2015-08-14)

Fixes not defaulting to `NODE_ENV=production` during runtime

## v79 (2015-08-10)

Supports WEB_CONCURRENCY for Performance-M dynos

## v78 (2015-07-24)

Defaults node environment to 'production'; bugfixes

- Fix runtime signature cache invalidation
- Provide error messaging for un-downloadable binaries
- Default to NODE_ENV=production for both build and runtime
- https://github.com/heroku/heroku-buildpack-nodejs/issues/60

## v77 (2015-07-15)

Npm bootstrapping skipped when using iojs.

- Fixes https://github.com/heroku/heroku-buildpack-nodejs/issues/202

## v76 (2015-06-23)

Refactor to bring caching logic to the forefront.

- Fixes cachDirectories issues
- Addresses https://github.com/heroku/heroku-buildpack-nodejs/pull/231
- Addresses https://github.com/heroku/heroku-buildpack-nodejs/issues/226
- Simplifies detect (package.json required)

## v75 (2015-04-24)

Updated build failure and help messaging.

## v74 (2015-04-24)

Updated messaging.

## v73 (2015-04-24)

Disables cache restoration if node_modules already exists.

## v72 (2015-04-23)

Accepts `cacheDirectories` array in package.json to override default `node_modules` caching.

- Documented at https://devcenter.heroku.com/articles/nodejs-support#cache-behavior
>>>>>>> a8cf29acf1f260261f4680001eb2c41c6d3d2cef
