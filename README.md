# Default VScode configuration

## Font

[Font installation](https://github.com/tonsky/FiraCode/wiki/VS-Code-Instructions)

```
"editor.fontFamily": "Fira Code, Menlo, Monaco, 'Courier New', monospace",
"editor.fontLigatures": true,
"editor.fontWeight": "400"
```

## Prettier config

```
{
  "trailingComma": "es5",
  "singleQuote": true,
  "printWidth": 100,
  "tabWidth": 2
}
```

# Snippets

## JS / TSX

```
{
	"Print to console": {
		"prefix": "clog",
		"body": [
			"console.log('$1', $1);"
		],
		"description": "Log output to console"
	},
	"Cray console": {
		"prefix": "cclog",
		"body": [
			"console.log('======================================================');",
			"console.log('$1', $1);",
			"console.log('======================================================');",
		],
		"description": "Scream log output to console"
	},
	"Ref": {
		"prefix": "ref",
		"body": [
				"ref={c => (this.$1 = c)}$0",
		],
		"description": "Add ref to component"
	},
	"React comp": {
		"prefix": "rf",
		"body": [
				"import React from 'react';",
				"",
				"function $1() {",
				"  return $2;",
				"}",
				"",
				"export default $1;",
		],
		"description": "Create functional component"
	},
	"import style": {
		"prefix": "ims",
		"body": "import style from './${TM_FILENAME_BASE/^(.)(.+)/${1:/downcase}$2/}.scss';",
		"description": "Style import shorthand"
	},
	"import style module": {
		"prefix": "imsm",
		"body": "import style from './${TM_FILENAME_BASE/^(.)(.+)/${1:/downcase}$2/}.module.scss';",
		"description": "Style module import shorthand"
	},
	"import clsx": {
		"prefix": "imcl",
		"body": "import cslx from 'clsx';",
		"description": "Clsx import shorthand"
	}
}
```

## TS

```
{
  "Print to console": {
		"prefix": "clog",
		"body": [
			"console.log('$1', $1);"
		],
		"description": "Log output to console"
	},
  "Cray console": {
		"prefix": "cclog",
		"body": [
			"console.log('======================================================');",
			"console.log('$1', $1);",
			"console.log('======================================================');",
		],
		"description": "Scream log output to console"
	},
}
```
