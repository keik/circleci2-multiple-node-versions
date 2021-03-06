circleci2-multiple-node-versions
====
Sample project to build with multiple Node.js versions in CircleCI 2.1!

[![build status][circleci-image]][circleci-url]
![Node.js Version Support][node-version]

## Branches

- [npm](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/npm)
- [npm-with-test-report](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/npm-with-test-report)
- [yarn](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/yarn)
- [yarn-with-test-report](https://github.com/teppeis-sandbox/circleci2-multiple-node-versions/tree/yarn-with-test-report)

Note: `npm` and `npm-with-test-report` uses `package-lock.json` introduced by npm@5.
So the lock file is ignored in npm@3 and 4 (v6 bundles npm@3 by default).

## How to use

1. Copy `.circleci/config.yml` to your project
2. [Add your project to CircleCI](https://circleci.com/docs/2.0/first-steps/)
3. Enable CircleCI 2.1 in Build Settings > Advanced Settings
4. Add a new "Environment Variables" in Build Settings > Environment Variables
    - name: `CIRCLE_CACHE_VERSION`, value: `20180123`
5. Rebuild

## License

MIT License: Teppei Sato &lt;teppeis@gmail.com&gt;

[circleci-image]: https://circleci.com/gh/teppeis-sandbox/circleci2-multiple-node-versions.svg?style=shield
[circleci-url]: https://circleci.com/gh/teppeis-sandbox/circleci2-multiple-node-versions
[node-version]: https://img.shields.io/badge/Node.js%20support-v6,v8,v10-brightgreen.svg
