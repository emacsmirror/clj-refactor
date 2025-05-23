# Changelog

## Unreleased

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.11.0/CHANGELOG.md#3110).

## 3.12.0

- `clean-ns` will now also reformat the `ns` form for whitespace-only changes, if needed.
  - Previously, this wasn't possible since refactor-nrepl generally only works at the structural level.
- Use refactor-nrepl [3.10.0](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.10.0/CHANGELOG.md#3100).

## 3.11.3

- Fix incorrectly serialized values for `cljr-slash` when using `cljr-suggest-libspecs`.

## 3.11.2

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.9.1/CHANGELOG.md#391).
  - Fixes https://github.com/clojure-emacs/clj-refactor.el/issues/556

## 3.11.1

* [#555](https://github.com/clojure-emacs/clj-refactor.el/pull/555): expand default `cljr-magic-require-namespaces` aliases.
* [#555](https://github.com/clojure-emacs/clj-refactor.el/pull/555): Handle an edge case for `cljr-slash`.

## 3.11.0

* [#554](https://github.com/clojure-emacs/clj-refactor.el/pull/554): Enable `cljr-slash-uses-suggest-libspec` by default.

## 3.10.0

* [#552](https://github.com/clojure-emacs/clj-refactor.el/issues/552): support TRAMP connections.

## 3.9.4

* Fix `cljr-version`.

## 3.9.3

* Internal: avoid the use of deprecated Elisp functions.

## 3.9.2

* [#523](https://github.com/clojure-emacs/clj-refactor.el/issues/523): Increase `js/` namespace detection accuracy for .cljc files.
* [#517](https://github.com/clojure-emacs/clj-refactor.el/issues/517): Remove `pkg-info` dependency.

## 3.9.1

* [#430](https://github.com/clojure-emacs/clj-refactor.el/issues/430) `cljr-add-missing-libspec`: produce more friendly prompts.
* `cljr-add-missing-libspec`: don't suggest members that are already interned into the current namespace.
  * e.g. the class `Thread` or the var `+` are already interned by default in Clojure namespaces, so they are redundant to suggest or insert into the `ns` form.

## 3.9.0

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.9.0/CHANGELOG.md#390).

## 3.8.0

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.8.0/CHANGELOG.md#380).
- Restore Emacs 26 compatibility.

## 3.7.1

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.7.1/CHANGELOG.md#371).

## 3.7.0

- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.7.0/CHANGELOG.md#370).
- [#537](https://github.com/clojure-emacs/clj-refactor.el/issues/537): Fail early in `cljr-rename-symbol` in case narrowing is in effect.

## 3.6.1

- Add the [clojure.math namespace](https://clojure.github.io/clojure/clojure.math-api.html) to magic requires (new with Clojure 1.11.0)

## 3.6.0

- [#532] Introduce `cljr-slash-uses-suggest-libspec` to use the language context aware `suggest-libspec` middleware for alias to libspec suggestions.
- [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.6.0/CHANGELOG.md#360).

## 3.5.6

* [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.5/CHANGELOG.md#355).

## 3.5.5

* [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.4/CHANGELOG.md#354).

## 3.5.4

* [Upgrade refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.3/CHANGELOG.md#353).

## 3.5.3

* Upgrade `cider`, `parseedn` and `inflections` dependencies.

## 3.5.2

* Use refactor-nrepl [3.5.2](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.2/CHANGELOG.md#352).

## 3.5.1

* Use refactor-nrepl [3.5.1](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.1/CHANGELOG.md#351).

## 3.5.0

* Use refactor-nrepl [3.5.0](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.5.0/CHANGELOG.md#350).
* Improve integration with Clojure 1.11's new `:as-alias` namespace directive.
  * Closes [#515](https://github.com/clojure-emacs/clj-refactor.el/issues/515), [#515](https://github.com/clojure-emacs/clj-refactor.el/issues/516)

## 3.4.3

- Use refactor-nrepl [3.4.2](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.4.2/CHANGELOG.md#342).

## 3.4.2

- [#514](https://github.com/clojure-emacs/clj-refactor.el/issues/514): cljr-slash: Fix `Wrong type argument: listp`.
- Use refactor-nrepl [3.4.1](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.4.1/CHANGELOG.md#341).

## 3.4.1

- Introduce `cljr-suggest-namespace-aliases` defcustom.

## 3.4.0

- Use refactor-nrepl [3.4.0](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.4.0/CHANGELOG.md#340).
- [#512](https://github.com/clojure-emacs/clj-refactor.el/issues/512): Fix occasional :require` / `:require-macros` confusion in `cljr-slash`.

## 3.3.3

- Adapt `cljr--inject-jack-in-dependencies` to upstream changes in CIDER.

## 3.3.2

- Use refactor-nrepl [3.3.2](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.3.2/CHANGELOG.md#332).

## 3.3.1

- Use refactor-nrepl [3.3.1](https://github.com/clojure-emacs/refactor-nrepl/blob/v3.3.1/CHANGELOG.md#331).

## 3.3.0

- Use refactor-nrepl [3.3.0](https://github.com/clojure-emacs/refactor-nrepl/blob/6c599d22579886b834ca4b46fec45beb34abf2d8/CHANGELOG.md#330).

## 3.2.3

- Use refactor-nrepl [3.2.2](https://github.com/clojure-emacs/refactor-nrepl/blob/deploy-typo/CHANGELOG.md#322-2022-01-29).

## 3.2.0, 3.2.1, 3.2.2 (2021-11-16)

- [#504](https://github.com/clojure-emacs/clj-refactor.el/issues/504): Introduce `cljr-print-right-margin`, `cljr-print-miser-width` customization options which control the line wrapping of ns forms after formatting them (as performed after `clean-ns`, `rename-file-or-dir`, etc).

## 3.1.0 (2021-11-10)

- Use refactor-nrepl [3.1.0](https://github.com/clojure-emacs/refactor-nrepl/blob/a6b052809e6c2c8b077bf0ae4684e05af0a5f484/CHANGELOG.md#310-2021-11-09).
- [#139](https://github.com/clojure-emacs/clj-refactor.el/issues/139): avoid a repeated prompt when using `(cljr-project-clean)`.

## 3.0.0 (2021-10-25)

- [#483](https://github.com/clojure-emacs/clj-refactor.el/issues/483): Improve performance of `cljr-slash` when typing fraction literals.
- [#482](https://github.com/clojure-emacs/clj-refactor.el/issues/482): Add missing defgroup form.
- [#470](https://github.com/clojure-emacs/clj-refactor.el/issues/470): Choose `deps.edn` over `pom.xml` as project file.
- Introduce `cljr-insert-newline-after-require` option.
- Introduce `cljr-injected-middleware-version` option, allowing users to customize the [refactor-nrepl](https://github.com/clojure-emacs/refactor-nrepl) version to be used.
- Dropped support for Emacs 25 (to match upstream changes in CIDER).

## 2.5.1 (2021-02-16)

- [#442](https://github.com/clojure-emacs/clj-refactor.el/issues/442): Send nREPL-based paths instead of CIDER-based paths.
- [#465](https://github.com/clojure-emacs/clj-refactor.el/issues/465): Fix breakage in `cljr-rename-symbol`.
- Automatically namespace artifacts in `deps.edn`.

## 2.5.0 (2020-02-29)

- [#455](https://github.com/clojure-emacs/clj-refactor.el/pull/455): Added support for detecting shadow-cljs projects.
- [#402](https://github.com/clojure-emacs/clj-refactor.el/issues/402): `cljr-stop-referring`: do not alter strings.
- [#380](https://github.com/clojure-emacs/clj-refactor.el/issues/380): `cljr-clean-ns`: fix `FileNotFoundException`, by trying both the absolute path and the path relative to the project root. This requires a new refactor-nrepl, old versions will only check the absolute path.

## 2.4.0 (2018-08-26)

- Compatible with CIDER 0.17 and 0.18.
- Hotload dependency temporarily disabled to make the middleware run on Java 10.
- Dropped support for Emacs < 25.1 (to match clojure-mode and CIDER).
- [#426](https://github.com/clojure-emacs/clj-refactor.el/issues/426): New variable, `cljr-middleware-ignored-paths`, to make the middleware ignore certain paths.
- [#408](https://github.com/clojure-emacs/clj-refactor.el/pull/408): New `cljr-before-warming-ast-cache-hook`, `cljr-after-warming-ast-cache-hook` callbacks around AST warming.
- [#394](https://github.com/clojure-emacs/clj-refactor.el/issues/394): New config option `cljr-assume-language-context`: by default, when clj-refactor encounters an ambiguous context (clj vs cljs) it creates a popup asking user which context is meant. If this option is changed to "clj" or "cljs", clj-refactor will use that as the assumed context in such ambigous cases.
- [#391](https://github.com/clojure-emacs/clj-refactor.el/issues/391): Prevent refactor-nrepl from being injected when starting a REPL outside a project, and add an option `cljr-suppress-outside-project-warning` to suppress the resultant warning.

## 2.3.1 (2017-07-04)

- [#363](https://github.com/clojure-emacs/clj-refactor.el/issues/363) cljr-favor-prefix-notation by default is set to false
- Display keymap bindings in documentation for minor mode
- New config setting `cljr-libspec-whitelist` to prevent libspecs which appear unused but are side-effecting at load from being pruned.
- [#301](https://github.com/clojure-emacs/clj-refactor.el/issues/301): `ad`  has gained a prefix to declare the symbol under the cursor.
- [#312](https://github.com/clojure-emacs/clj-refactor.el/issues/312): Allow `sut` alias to be customized.
- [#305](https://github.com/clojure-emacs/clj-refactor.el/issues/305): Don't call lookup-alias for non namespaced keywords at all when slash is typed. However trigger lookup alias with the leading :: stripped off the prefix if the keyword is namespaced.
- Require a custom test framework for Clojurescript test files. By default it's `cljs.test` but it can be customized with `cljr-cljs-clojure-test-declaration`.

### Changes

- [#302](https://github.com/clojure-emacs/clj-refactor.el/issues/302): `ad` now understands def-like things, e.g. defs created by Schema.
- When inserting ns form to blank clojure-ish file, check if cider is available and connected for better detecting the expected namespace.
- Remove the warning about missing nREPl ops.
- Remove threading macro related features because they are moved to Clojure mode. However, the usual mnemonics for these features still work only they reference the Clojure mode implementations.
- Remove cycle privacy, cycle if and cycle collection type features. They are moved to Clojure mode. The usual mnemonics for cycle privacy and cycle if features still work only they refer the Clojure mode implementations. Cycle collection type got reworked into convert collection to list, quoted list, map, vector and set. *Cycle* collection type is no longer supported.
- Compatible with clojure-mode 5.6.1 and above.
- Remove *most* of the code implementing `let` related refactorings because these featured got migrated and reworked in Clojure mode. The usual mnemonics for these features still work and also a version of these features using multiple cursors are still maintained here as multiple cursors mode is not supported in Clojure mode.
- [#294](https://github.com/clojure-emacs/clj-refactor.el/issues/294): Remove dash library dependency.
- [#372](https://github.com/clojure-emacs/clj-refactor.el/issues/372): Remove s.el dependency

### Bugs fixed

- [#368](https://github.com/clojure-emacs/clj-refactor.el/issues/368): Fix inline symbol fails on inlining composed function in a `def`
- [#299](https://github.com/clojure-emacs/clj-refactor.el/issues/299): `ml` moves cursor
- [#309](https://github.com/clojure-emacs/clj-refactor.el/issues/309): `am` creates alias for fully-qualified symbols.
- [#313](https://github.com/clojure-emacs/clj-refactor.el/issues/313): teach `pf` about function literals using `%&`.
- [#320](https://github.com/clojure-emacs/clj-refactor.el/issues/320): `*data-readers*` ignored when searching for macros.
- [#339](https://github.com/clojure-emacs/clj-refactor.el/issues/339): Teach stop refer to understand multiline refer clauses.
- [#341](https://github.com/clojure-emacs/clj-refactor.el/issues/341): Avoid creating circular dependencies with move form when source namespace refers to the target namespace with a require.
- [refactor-nrepl#183](https://github.com/clojure-emacs/refactor-nrepl/issues/183) Applied conversion between Unix-like path generated by Emacs under Cygwin and Windows-like path required by nREPL. Cider functions `cider-to-nrepl-filename-function` and `cider-from-nrepl-filename-function` are used.
- Fix `cljr--normalize-symbol-name` when the symbol name starts with `#'`.
- [#371](https://github.com/clojure-emacs/clj-refactor.el/issues/371): Stop `cljr-slash` messing up `(in-ns ...)` forms

## 2.2.0 (2016-03-22)

- Smarten up `cljr-stop-referring` to replace `:refer :all` style require with alias and apply the alias to all occurrences of symbols from the referred namespace.
- [#292](https://github.com/clojure-emacs/clj-refactor.el/issues/292): The buffer wasn't saved after adding a missing libspec causing clean-ns
to act on stale data.
- Don't try to resolve `js/` in cljs-mode
- `cljr-create-fn-from-example` improvements: strip ns off keywords when making param name; always include a blank line over new function
- [#306](https://github.com/clojure-emacs/clj-refactor.el/issues/306): Add-require doesn't jump back if there is no REPL connection with refactor-nrepl configured

### Changes

- Compatible with CIDER 0.11
- Follow up CIDER 0.11 injecting its own dependencies at `cider-jack-in` by adding clj-refactor's own dependencies to the approriate vars in CIDER. Both leiningen and boot are supported. Set `cljr-inject-dependencies-at-jack-in` to nil to opt out.

## 2.0.0 (2016-02-06)

- [#267](https://github.com/clojure-emacs/clj-refactor.el/issues/267):
 Add `cljr-require-macro` which requires a macro into the current
 namespace.
- Add prefix variant to `cljr-add-import-to-ns` for insertion of imports in the cljs part of the ns declaration.
- Add prefix variant to `cljr-add-use-to-ns` for insertion of 'use' in the cljs part of the ns declaration.
- Add prefix variant to `cljr-add-require` for insertion of requires in the cljs part of the ns declaration.
- Boot support for `cljr-clean-ns`.
- Boot support for `cljr-sort-project-dependencies`.
- Boot support for `cljr-update-project-dependencies`.
- Boot support for `cljr-update-project-dependency`.
- [#228](https://github.com/clojure-emacs/clj-refactor.el/issues/238): Boot support for `cljr-add-project-dependency`.
- Get rid of `cljr-reload-config`.  We're now sending the configuration options down to the middleware on each request instead of storing it down there.
- Make magic requires cljc aware.
- [#215](https://github.com/clojure-emacs/clj-refactor.el/issues/215): Improve the magic requires feature (when you hit `/`) by asking the middleware for all available namespace aliases.
- Add `cljr-extract-def` which extracts the form at, or around, point as a def.
- Add `cljr-change-function-signature` to re-order or re-name function parameters.
- Keep pressing `l` after `cljr-expand-let` to expand further.
- [refactor-nrepl#99](https://github.com/clojure-emacs/refactor-nrepl/issues/99): if cljr-thread-first-all or cljr-thread-last-all is called with a prefix the last expression is not threaded. cljr-thread-all-but-last defcustom has the same effect without the prefix
- [hydra](https://github.com/abo-abo/hydra) menus for discoverability: they help to (re)learn clj-refactor key bindings. See: [parent hydra](https://github.com/clojure-emacs/clj-refactor.el/wiki/Hydra).

### Bugs fixed

- [#285](https://github.com/clojure-emacs/clj-refactor.el/issues/285): clean-ns did the wrong thing unless the code was loaded.

### Changes

- [#265](https://github.com/clojure-emacs/clj-refactor.el/issues/265): Feedback to the user is lost among other general messages from emacs.
- Make `cljr-clean-ns` the only default function used by `cljr-project-clean`.
- Remove `cljr-remove-unused-requires` which is replaced by `cljr-clean-ns`.
- Remove `cljr-replace-use` which is replaced by `cljr-clean-ns`.
- Remove `cljr-sort-ns` which is replaced by `cljr-clean-ns`.
- `cljr-remove-debug-fns` has been removed.
- `cljr-magic-require-namespaces` is now only consulted in the event the namespace alias isn't already used in the project.
- [#217](https://github.com/clojure-emacs/clj-refactor.el/issues/217): When requiring the test framework in test files stop favoring `:refer :all`.
- [#217](https://github.com/clojure-emacs/clj-refactor.el/issues/217): Add a bunch of defcustoms to parameterise what gets inserted into the test namespaces for the various test frameworks.
- [#216](https://github.com/clojure-emacs/clj-refactor.el/issues/216): Teach our automatic ns generator about cljc files.
- Teach `cljr-extract-constant` about the `^:const` hint to the compiler.
- Use yasnippet for placeholder parameters in `cljr-create-fn-from-example`
- Highlight the function be promoted with overlays in `cljr-promote-function`.
- Highlight the form to be extracted with overlays in `cljr-extract-function`.
- `cljr-create-fn-from-example` is now significantly smarter about guessing parameter numbers and names.
- `cljr-sort-ns` no longer marks the buffer as changed if it did no work.
- `cljr-rename-symbol` now fails earlier, before prompting the user for a new name if an AST can't be built due to errors.
- support for emacs 24.3 and older is dropped
- [refactor-nrepl#85](https://github.com/clojure-emacs/refactor-nrepl/issues/85): Eliminate some find usages duplicates
- Some AST based features (find usages, rename symbol, inline symbol) ignore namespaces that cannot be analyzed if `cljr-ignore-analyzer-errors` set to true instead of failing entirely.
- By default warning is given when AST based feature is used and clj-refactor only proceeds with it if the user allowed evalling the project as the analyzer also evals first level forms. To disable the warning set `cljr-warn-on-eval` to `nil`. This also reenables warming AST cache at startup of the REPL.

## 1.1.0 (2015-07-06)

- Add `cljr-describe-refactoring` which shows the wiki page describing one of the available refactorings inline in emacs.
- Add `cljr-rename-file-or-dir` to replace `cljr-rename-file`.
- Add `cljr-inline-symbol` which replaces the symbol at point with its definition.
- Add `cljr-add-stubs` which adds a skeleton implementation of the protocol or interface at point.
- Add `cljr-reify-to-defrecord`
- Add `cljr-show-changelog` so users don't have to visit github to find out what's changed after a package update.
- Add `cljr-create-fn-from-example` to create function stub based on example usage
- Add `cljr-update-project-dependencies` (for leiningen only) prompts to update dependencies in project.clj, listing available versions
- Now `cljr--add-test-use-declarations` actually checks the file system in order to find its require for the source ns.
- Improvements to error handling and reporting around analyzing namespaces
- Configuration option `cljr-find-usages-ignore-analyzer-errors`: when true, find-usages will run even if there are compilation/analyzer problems in some namespaces; defaults to nil.
- Configuration option `cljr-favor-private-functions`: set to nil to create public functions where applicable.
- Better support for `cljr-use-metadata-for-privacy` when creating functions.
- Highlight the relevant form when extracting and promoting functions.
- Multiple cursors is used when extracting and promoting functions (disable by setting `cljr-use-multiple-cursors` to nil)
- Not using multiple-cursors when in evil-mode.

## 1.0.5 (2015-05-02)

- Add `cljr-reload-config` to resubmit config settings to the middleware
- Add config setting for `clean-ns` to not do rewriting to favor prefix form.
- Add `cljr-extract-function`
- Add `cljr-hotload-dependency`
- Hotloading of artifacts added with `cljr-add-project-dependency`
- Add `cljr-remove-let`
- Add `cljr-clean-ns`
- Add `cljr-add-missing-libspec`
- Add `cljr-promote-function`
- Add `cljr-find-usages`
- Add `cljr-rename-symbol`

## 0.13 (2014-11-19)

- Removed `cljr-cycle-stringlike`.  This function was duplicating the functionality of `clojure-mode`s `clojure-toggle-keyword-string`
- Add `cljr-cycle-if`
- Common namespace shorthands are (optionally) automatically required when you type it.
- Comparator for sort require, use and import is configurable, add optional lenght based comparator to sort longer first
- Add semantic comparator to sort items closer to the current namespace first
- Add `cljr-project-clean` with configurable clean functions
- Add `cljr-sort-project-dependencies`
- Add `cljr-add-project-dependency`
- Add `cljr-remove-debug-fns`
- performance tweak for `cljr-remove-unused-requires` if `refactor-nrepl` is used

## 0.12 (2014-03-03)

- When expanding let, or moving expressions to let, it now replaces
  duplicates in the let body with the bound name.

## 0.11 (2014-02-20)

- Add `cljr-raise-sexp`
- Add `cljr-remove-unused-requires`
- Add `cljr-move-form`

## 0.10 (2014-01-30)

- Add `cljr-stop-referring`
- Add `cljr-destructure-keys`
- Add `cljr-sort-ns`

## 0.9 (2014-01-26)

- Add `cljr-replace-use`
- Add `cljr-add-declaration`

## 0.8 (2014-01-20)

- Add `cljr-cycle-stringlike`
- Add `cljr-cycle-coll`
- Add `cljr-cycle-privacy`

## 0.7 (2014-01-15)

- Add `cljr-thread-first-all`, `cljr-thread-last-all` and `cljr-unwind-all`

## 0.6 (2014-01-11)

- Add `cljr-move-to-let`
