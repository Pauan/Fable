### 1.0.0-narumi-909

* Test

### 0.7.49

* Fix #744: CLI argument flags

### 0.7.48

* Fix #736: Case testing with erased unions

### 0.7.47

* Tailcall optimizes function arguments: #681

### 0.7.45

* Fix import expressions with methods with function arguments: #721

### 0.7.43

* Add reflection methods (see ReflectionTests.fs)
* Improve import expressions #721

### 0.7.42

* Tailcall optimizations: PR #669 + Fixes

### 0.7.37

* Add FSharp.Core.dll to fable-compiler package
* Improve handling of `jsThis`

### 0.7.35

* Only show Rollup warnings in `--verbose` mode
* Minor fixes

### 0.7.34

* Fix #660: `Option.fold` and `Option.foldBack`

### 0.7.33

* Add operator `enum`

### 0.7.32

* Fixed default comparer: PR #658

### 0.7.31

* Added BigInt conversions: PR #650

### 0.7.30

* Fix #649: Int64 serialization
* Fix #648: Caching of namespace F# entities
* Fix #646: Zero fill shift right (>>>) for uint32

### 0.7.29

* Add `BigInteger` support

### 0.7.28

* Fix #640: Omitted non optional nulls
* Fix #638: Inlined methods with `this` argument

### 0.7.27

* Add `--includeJs` compiler argument
* Fix #629: Visual Studio error format
* Fix  #637: IEnumerable runtime issue

### 0.7.26

* Fixed Option.foldBack (#634)
* Improve .NET Enumerator/JS Iterator compatibility
* Fix #633: jsThis
* Fixed Option.foldBack (PR #634)

### 0.7.25

* Fix #623: JS Global properties
* Fix #624: Aether compilation

### 0.7.24

* Fix module generic methods without arguments
* Added `String.IndexOfAny/Compare/Equals` with `StringComparison` enum
* Fix generic types when compiling to ES2015
* Unify `Equals` and `CompareTo` methods of `Long.ts`

### 0.7.23

* Fix #348 #608 Double/Int32 Parse & TryParse
* Fix #609: Event unsubscription
* Fix custom exception type testing in ES5
* Inline local lambdas as values (#601)
* Fix edge case in `toJson` (#611)
* Fix fable-core Babel compilation
* Added 64-bit integers (#600)
* Fix #237: Recursive value definitions
* Added char to int (#594)

### 0.7.22

* Fix secondary constructors of imported classes
* Improvements in option handling

### 0.7.20

* Prevent infinite loops for bundle errors in watch mode

### 0.7.19

* Fix #509: Add KeyValuePattern
* Fix #544 #585: Bundling in watch mode
* Fix #589: Regex Provider with Fable 0.7
* Add optional argument to GlobalAttribute

### 0.7.18

* Add validation to `ofJson`
* Make `Assert.AreEqual` work with F# equality
* Improve dynamic programming (add `jsThis`)
* Add `Printf.kprintf` (#583)
* Fix sprintf "%X" (#580)
* Fix #579: Printf.printfn

### 0.7.17

* Add `Pojo` union types

### 0.7.16

* Fix issues in generic resolution

### 0.7.15

* Issue warning when calling `typeof` on a generic parameter
* Use absolute paths for assembly references in `node_modules`

### 0.7.14

* Use "umd" distribution of fable-core and other libs when compiling for umd modules
* Fix #569: Types with circular dependencies

### 0.7.12

* Fix #568: Types with `StructAttribute` (compiled as records)
* Better checking when calling functions with `PassGenericsAttribute`

### 0.7.11

* Some adjustments in attribute resolution

### 0.7.10

* Fix #565, #566: Only watch F# files
* Fix #564: Don't overload methods from imported classes
* Fix #563: Overloads with `PassGenericsAttribute`

### 0.7.9

* Fix `Array.rev` (see #559)
* Added UnboxFast intrinsic / List.truncate (see #561)

### 0.7.8

* `System.Exception` translates to JS `Error`
* Fix #556: inline methods placed after calls

### 0.7.7

* Fix ES2015 imports

### 0.7.6

* Too many changes to be listed, check the [migration guide](http://fable.io/blog/Introducing-0-7.html)

### 0.7.5-alpha.41

* Fix cyclic dependencies in fable-core

### 0.7.5-alpha.40

* Minor fix

### 0.7.5-alpha.39

* Simplify Reflection system
* Add `PojoAttribute`
* Replace baseDir of references with --refs argument

### 0.7.5-alpha.38

* Fix #547: Ignored entities conflicting when calculating root namespace

### 0.7.5-alpha.37

* Mangle class methods when they conflict with an implemented interface

### 0.7.5-alpha.35

* Fix #545: Using `Microsoft.FSharp` namespace

### 0.7.5-alpha.34

* Add `import: selector->path->'T` to import expressions
* Make arguments of JsConstructor statically typed
* Add logs when compiling files for bundling

### 0.7.5-alpha.33

* Fix default watch directories
* Ignore interfaces

### 0.7.5-alpha.32

* Compile scripts referenced as plugins
* Apply Replace plugins to any call
* Include in compilation JS files with relative paths

### 0.7.5-alpha.31

* Fix #535: Script referenced entity replacements

### 0.7.5-alpha.30

* Allow configuration of watching dirs

### 0.7.5-alpha.29

* Fix infinite recursion when resolving generic parameters

### 0.7.5-alpha.28

* More meaningful runtime representation of non-declared types

### 0.7.5-alpha.27

* When inlining, assign arguments referenced more than once to a temp var
* `Array.zeroCreate` fills non-numeric arrays with null

### 0.7.5-alpha.26

* Resolve trait calls as normal method calls (check EmitAttribute, etc)

### 0.7.5-alpha.24

* Fix mangled interfaces
* Improve error messages

### 0.7.5-alpha.23

* Add `MangleAttribute` to prevent conflicts with interfaces
* Allow combination of `ImportAttribute` and `EmitAttribute`
* Several fixes

### 0.7.5-alpha.22

* Add catch-all for missing replacements when referencing
  types of the BCL or FSharp.Core
* Omit `.js` extension again in imports to keep
  compatibility with Require.js

### 0.7.5-alpha.21

* Don't print warnings in process.stderr (see #516)
* Add `String/formatError` (see #519)
* Add `.js` extension to `fable-core` and internal imports

### 0.7.5-alpha.19

* Distribute fable-core with ES2015 (default) and UMD module formats

### 0.7.5-alpha.18

* Don't deem interface setters as overloads (see #505)

### 0.7.5-alpha.17

* Update FCS and use Forge to read .fsproj files (removes MSBuild dependency)
* Bug fixes and optimizations

### 0.7.5-alpha.16

* Add JsFunc and JsCons to Fable.Core.JsInterop

### 0.7.5-alpha.15

* Use outDir to place the generated dll with .fsproj projects
* Only emit warnings when generating dlls in verbose mode
* Fix error when reading Rollup options

### 0.7.5-alpha.14

* Fix errors in Fable JS API

### 0.7.5-alpha.12

* Change `--bundle` option to `--rollup`
* `--rollup` can accept an object (in fableconfig.json) with Rollup config
* Improve plugin resolution for Babel and Rollup

### 0.7.5-alpha.11

* Add a block scope to switch cases (see #483)

### 0.7.5-alpha.10

* Fix invalid identifiers in top level members (see #482)
* Generate `dll` also for `fsproj` files
* Expose Fable library to JS API

### 0.7.5-alpha.9

* Fix issues with bundling and `System.Exception`

### 0.7.5-alpha.8

* Fix problems with `dll` generation

### 0.7.5-alpha.7

* Add experimental `--dll` compiler option to generate assemblies

### 0.7.5-alpha.6

* Fix path resolution when referencing assemblies

### 0.7.5-alpha.5

* Fix partial patterns not returning any value (see #478)

### 0.7.5-alpha.4

* Minor fixes

### 0.7.5-alpha.2

* Resolve relative paths of referenced projects/dlls as
  if they were pointing to generated JS code from the fsproj/dll file
  (`EntryModuleAttribute`) or from working directory (`--refs`)
  and make them reachable from `outDir` (see #472)
* Always resolve relative paths in command line options with
  the directory from where fable is called

### 0.7.5-alpha.1

* Fix prerelease semver. See: https://docs.npmjs.com/misc/semver#prerelease-tags

### 0.7.5-alpha

* Add `typedefof<>`, `.IsGenericType`, `.GetGenericTypeDefinition`

### 0.7.4-alpha

* Resolve import relative paths so they can be reached from `outDir`
  if they don't point to an internal file (see #472)

### 0.7.3-alpha

* Add warning when creating references of types unknown at compile time

### 0.7.2-alpha

* Convert functions to delegates when passed as arguments to EmitAttribute
* Add warning when passing generic param to Serialize.ofJson/inflate

### 0.7.1-alpha

* Add `--bundle` compiler option
* Bring back JSON serialization with `$type` info

### 0.7.0-alpha

* Add type info to JS constructors: cases (unions) and properties (records and classes)
* Extend type references with generic info when calling `typeof`
* Add `GenericParamAttribute` to implicitly pass type info of generic parameters
* Add `MutatingUpdateAttribute` to compile record updates as mutations
* Add `EntryModuleAttribute` to mark assemblies as Fable libraries

### 0.6.15

* Revert change from 0.6.14: ES6 modules automatically enable
  strict mode, so the directive is not needed

### 0.6.14

* Add always "use strict" directive

### 0.6.12

* Now fableconfig.json can be in JSON5 format (comments!)
* Omit lambda argument when it's of unit type

### 0.6.11

* Don't wait until "postbuild-once" script is finished (see #432)

### 0.6.9

* Fix #431: Add --babelrc compiler option
* Fix #432: Add "postbuild-once" script
* Fix #433: Add --noTypedArrays compiler option
* Fix #436: Inform users about not supported overloads of String.IndexOf/LastIndexOf
* Fix #438: Incorrect this in local let functions creating object expressions
* Fix #439: IDE locking project file and preventing watch compilations
* Change compilation defaults: module=commonjs & loose=true

### 0.6.7

* Fix #416: Can't ifdef around a load directive
* Fix List.unfold: PR #428
* Use reference hint paths for netcore: PR #423

### 0.6.6

* Support ResizeArray.FindAll: PR #412

### 0.6.5

* Support decimal (converted to JS number): PR #413
* Support recursive records: PR #417

### 0.6.4

* Fix #411: for .. downto

### 0.6.3

* Fix watch compilation on Windows

### 0.6.2

* Integer conversions (see #407)

### 0.6.1

* Multiple bug fixes
* Internal Fable AST additions
* [Rewrite plugins](https://fable-compiler.github.io/docs/plugins.html#Creating-rewriter-plugins)
* Use let/const when compiling value bindings to ES6
* Compile pattern matching with string or number literals as switch statements

### 0.5.11

* Fix #382 (partially): Exclude files in "node_modules" when calculating the base
  directory of referenced dlls.

### 0.5.10

* Fix #369: Extra blank lines when running postbuild script
* Fix #375: Add warning when replacements change semantics (printf, Async.Start...)
* Fix #377: Remove null args at the end of method/constructor calls also with macros

### 0.5.9

* Fix type testing with Erased Unions
* Erase assigments generated for tuple, record and union gets
* Fix #370: Add warning when using unions or records with Dictionary (as keys) or HashSet
* Internal cleanup

### 0.5.8

* Use chokidar to watch for file changes
* Fix calculation of relative paths with special characters (like "#")
