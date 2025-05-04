

### Terminal Integrado
```json
  /* Oculta abas quando tem um único terminal */
  "terminal.integrated.tabs.hideCondition": "singleTerminal",

  /* Matar terminal quando fechar VScode */
  "terminal.integrated.persistentSessionReviveProcess": "never",

  /* Remove 'desenhos' da margem do terminal */
  "terminal.integrated.shellIntegration.decorationsEnabled": "never",

  /* Shell de cada SO */
  "terminal.integrated.defaultProfile.linux": "zsh",
  "terminal.integrated.defaultProfile.osx": "zsh",
  "terminal.integrated.defaultProfile.windows": "PowerShell",
  // "terminal.integrated.defaultProfile.windows": "Git Bash",
  // "terminal.integrated.defaultProfile.windows": "Ubuntu-20.04 (WSL)",

  /* Fonte do terminal */
  "terminal.integrated.fontFamily": "CaskaydiaCove NF",
  "terminal.integrated.fontSize": 14,
  "debug.console.fontSize": 10,

  "terminal.integrated.gpuAcceleration": "off",
```

### Interface do VS Code
```json
  "update.mode": "start",
  
  /* Abre VScode vazio */
  "workbench.startupEditor": "nome",
  "workbench.editor.untitled.hint": "hidden",

  /* Caminho do arquivo nas abas */
  "breadcrumbs.enabled": false,
  "workbench.editor.labelFormat": "short",

  /* Temas */
  "workbench.colorTheme": "Omni",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.productIconTheme": "fluent-icons",

  /* Comportamento Explorador */
  "window.menuBarVisibility": "visible",
  "explorer.compactFolders": false,
  "explorer.confirmDragAndDrop": true,
  "explorer.confirmDelete": false,

  /* Trocar ícones de arquivos */
  "files.associations": {
    ".sequelizerc": "javascript",
    ".stylelintrc": "json",
    ".prettierrc": "json",
    "*.tsx": "typescriptreact",
    ".env.*": "dotenv",
    ".env": "dotenv"
  },
  
  /* Arquivos e diretórios ocultos no explorador */
  "files.exclude": {
    "**/.git": false,
    "**/.svn": true,
    "**/.hg": true,
    "**/CVS": true,
    "**/.DS_Store": true,
    "**/node_modules": false
  },

```

### Editor de texto
```json
  "editor.tabSize": 2,
  "editor.fontSize": 16,
  "editor.lineHeight": 26,
  "editor.fontFamily": "Fira Code", //"JetBrains Mono"
  "editor.fontLigatures": true, //OK
  "editor.semanticHighlighting.enabled": false, //OK
  "editor.rulers": [80, 120],
  "editor.minimap.enabled": true,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": "active",
  "editor.parameterHints.enabled": false, //true
  "editor.renderLineHighlight": "gutter", //OK




```

### LINT
```json
  "editor.formatOnType": false,
  "editor.formatOnPaste": false,
  "editor.formatOnSave": false,
  "editor.codeActionsOnSave": { //OK
    "source.fixAll.eslint": true,
    "source.addMissingImports": true,
    "source.organizeImports": true
  },
  "eslint.format.enable": false,
  "eslint.validate": [ //OK
  "javascript",
  "javascriptreact",
  "graphql"
  ],
  "eslint.packageManager": "yarn",

  "[prisma]": {
    "editor.formatOnSave": true //OK
  },

  "[json]": {
    "editor.defaultFormatter": "vscode.json-language-features",
  },

  "[jsonc]": {
    "editor.defaultFormatter": "vscode.json-language-features",
  },

```


### Sugestões de Autocompletar
```json
  "emmet.syntaxProfiles": {
    "javascript": "jsx"
  }, //OK
  "emmet.includeLanguages": { //OK
    "javascript": "javascriptreact",
    "typescript": "typescriptreact",
    "javascriptreact": "javascriptreact",
    "typescriptreact": "typescriptreact"
  },
  "javascript.suggest.autoImports": true, //OK
  "typescript.suggest.autoImports": true, //OK
  "editor.snippetSuggestions": "inline", //OK
  "editor.suggestSelection": "first", //OK
  "editor.acceptSuggestionOnCommitCharacter": false, //OK
  "emmet.showSuggestionsAsSnippets": false, //OK
  "editor.suggest.showWords": true, //OK
  "extensions.ignoreRecommendations": true, //OK
  
  "tabnine.experimentalAutoImports": true, //OK
```

### DART e FLUTTER
```json
  "generate.template.type": "Clean Code",
  "dart.debugSdkLibraries": false,
  "dart.openDevTools": "never",
  "dart.showInspectorNotificationsForWidgetErrors": false,
  "dart.previewFlutterUiGuides": true,
  "dart.previewFlutterUiGuidesCustomTracking": true,
  "dart.lineLength": 85,
  "dart.hotReloadOnSave": "manualIfDirty",
  "dart.flutterHotReloadOnSave": "all",
  "[dart]": {
    "editor.formatOnSave": true,
    "editor.formatOnType": true,
    "editor.formatOnPaste": false,
    "editor.selectionHighlight": false,
    "editor.suggest.snippetsPreventQuickSuggestions": false,
    "editor.suggestSelection": "first",
    "editor.tabCompletion": "onlySnippets",
    "editor.wordBasedSuggestions": false
  }
```


## Extensões essenciais
```json
  /* DotENV */
  "dotenv.enableAutocloaking": false,

  /* GIT e similares */
  "gitlens.codeLens.recentChange.enabled": false, //OK
  "gitlens.codeLens.authors.enabled": false, //OK
  "gitlens.codeLens.enabled": false, //workbench.iconTheme
  
  "git.enableSmartCommit": true, //OK
  "git.openRepositoryInParentFolders": "always",
  "diffEditor.ignoreTrimWhitespace": false,

  /* Live Server e Live Share */
  "liveServer.settings.donotShowInfoMsg": true,
  "liveshare.featureSet": "insiders", //OK
  "liveshare.presence": true,
  "liveshare.audio.startCallOnShare": true,

  /* OUTRAS  */
  /* remover preview de cores para o modelo ARGB usado nas interfaces do Flutter */
  "color-highlight.languages": ["*", "!dart"],
  "sqlite.recordsPerPage": 20,
  // "importCost.bundleSizeDecoration": "both",
  
  
  /* DESATIVADAS */
  // "prettier.arrowParens": "always",
  // "prettier.bracketSpacing": true,
  // "prettier.semi": true,
  // "prettier.singleQuote": false,
  // "prettier.trailingComma": "all",
  
  // "codesnap.backgroundColor": "transparent",
  // "codesnap.transparentBackground": true,
  // "codesnap.boxShadow": "0 0 0",

  // "todo-tree.general.tags": [
  //   "BUG",
  //   "HACK",
  //   "FIXME",
  //   "TODO",
  //   "XXX",
  //   "[ ]",
  //   "[x]"
  // ],
  // "todo-tree.regex.regex": "(//|#|<!--|;|/\\*|^|^\\s*(-|\\d+.))\\s*($TAGS)",

  // "simple.readme.settings.github": "LeonardoFuba",
  // "simple.readme.settings.name": "Leonardo",
  // "simple.readme.settings.lang": "pt-BR",
```


### Material Icon Theme
```json
  "material-icon-theme.activeIconPack": "react",
  // "material-icon-theme.activeIconPack": "nest",
  // "material-icon-theme.activeIconPack": "angular",
  // "material-icon-theme.activeIconPack": "vue_vuex",
  "material-icon-theme.folders.theme": "specific",
  "material-icon-theme.folders.associations": {
    "adapters": "contract",
    "grpc": "pipe",
    "kube": "kubernetes",
    "main": "lib",
    "websockets": "pipe",
    "implementations": "core",
    "protos": "pipe",
    "entities": "class",
    "kafka": "pipe",
    "use-cases": "functions",
    "migrations": "tools",
    "schemas": "class",
    "useCases": "functions",
    "eslint-config": "tools",
    "typeorm": "database",
    "_shared": "shared",
    "mappers": "meta",
    "fakes": "mock",
    "modules": "components",
    "subscribers": "messages",
    "domain": "class",
    "protocols": "contract",
    "infra": "app",
    "view-models": "views",
    "presentation": "template",
    "dtos": "typescript",
    "http": "container",
    "providers": "include",
    "factories": "class",
    "repositories": "mappings",
    "unit": "serverless",
    "login": "secure",
    "splash": "ci",
    "integration": "ci"
  },

  "material-icon-theme.files.associations": {
    "knexfile.ts": "database",
    "ormconfig.json": "database",
    "tsconfig.json": "tune",
    "*.proto": "3d",
    "*.webpack.js": "webpack",
    ".prettierrc": "json",
    ".env": "key"
  },

  "material-icon-theme.languages.associations": {
    "dotenv": "tune"
  },
```

### Code Spell / Error Lens
```json
  "errorLens.exclude": ["Unknown word"],
  "cSpell.language": "en,pt", //OK
  "cSpell.enableFiletypes": [
    "!asciidoc",
    "!c",
    "!cpp",
    "!csharp",
    "!go",
    "!handlebars",
    "!haskell",
    "!jade",
    "!java",
    "!latex",
    "!php",
    "!pug",
    "!python",
    "!restructuredtext",
    "!rust",
    "!scala",
    "!scss"
  ],

  "cSpell.userWords": [
    "appbar",
    "chakra",
    "clsx",
    "dayjs",
    "fastify",
    "Fastify",
    "knexfile",
    "lcov",
    "middlewares",
    "prefetch",
    "readonly",
    "respawn",
    "rocketseat",
    "typeorm",
    "upsert",
    "Vite",
    "whatsapp",
    "wireframe"
  ],
```

### Outras configurações
```json
  "security.workspace.trust.untrustedFiles": "newWindow",
  "screencastMode.onlyKeyboardShortcuts": true, //OK
  "terminal.integrated.showExitAlert": false, //OK
  "editor.accessibilitySupport": "off", //OK
  "javascript.updateImportsOnFileMove.enabled": "always", //OK
  "typescript.updateImportsOnFileMove.enabled": "never", //OK
  "typescript.tsserver.log": "off", //OK
```