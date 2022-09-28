# SwiftLint

Central repository for [SwiftLint](https://github.com/realm/swiftlint) configurations to fetch in projects to keep a consistent style.

## Usage

Add a `.swiftlint.yml` file to the root of your project:

```yml
parent_config: https://raw.githubusercontent.com/Automattic/swiftlint-config/7e6dc750123b1fb41830f2e385c0414f9953b23d/.swiftlint.yml
remote_timeout: 10.0
```

You can further configure the `.swiftlint.yml` to override the settings fetched from here. For example:

```yml
parent_config: https://raw.githubusercontent.com/Automattic/swiftlint-config/7e6dc750123b1fb41830f2e385c0414f9953b23d/.swiftlint.yml
remote_timeout: 10.0

disabled_rules:
  - control_statement
```

Note that you SwiftLint supports hierarchical configurations. You can add a `.swiftlint.yml` to a subfolder and all and only the files in that subfolder will use the resulting settings.
