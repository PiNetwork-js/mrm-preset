# MMR Preset

Pinetwork-js preset for [mrm](https://github.com/sapegin/mrm) to easily init projects and keep configuration files in-sync.

### Getting started

```sh
npm install mrm @pinetwork-js/mrm-preset -D
# or with Yarn
yarn add mrm @pinetwork-js/mrm-preset -D
```

Add script to `package.json` file:

```json
{
	"scripts": {
		"mrm": "mrm --preset @pinetwork-js/mrm-preset"
	}
}
```

Run tasks:

```sh
npm run mrm all --interactive # or task1 task2 etc.
# or with Yarn
yarn mrm all --interactive # or task1 task2 etc.
```

`--interactive`, `-i` : to have the questions in an interactive way (instead of `--config:foo bar --config:foo1 bar1 etc.`).

### Available tasks

- **all** (alias) : runs respectively **license**, **gitignore**, **editorconfig**, **beauty**, **changelog**, **typescript** and **ci**
- **base** (alias) : runs respectively **license**, **gitignore**, **editorconfig**, **beauty** and **changelog**
- **beauty** : setups ESLint and Prettier
- **changelog**: setups a basic Changelog.md
- **ci** : setups GitHub Actions
- **editorconfig** : setups a EditorConfig file
- **gitignore** : setups a Gitignore file
- **license** : setups a MIT license
- **package** : setups a complete package.json file
- **release-please** : setups Release Please action
- **typescript** : setups TypeScript
