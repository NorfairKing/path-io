## Path IO 0.3.1

* Introduced synonym for `forgivingAbsence'` —
  `ignoringAbsence`. `forgivingAbsence'` is deprecated now, but it's still
  there.

* Added a handy shortcut `ensureDir` that is defined as
  `ensureDir = createDirIfMissing True`.

* Made `getHomeDir` and `getTempDir` more robust when they are influenced by
  values of environment variables.

## Path IO 0.3.0

* Added `forgivingAbsence`, `resolveFile`, and `resolveDir` functions, so
  the package now provides all functionality that `Path.IO` module in Stack
  has.

* Added closed type family `RelPath`, `makeRelative`, and
  `makeRelativeToCurrentDir` functions.

* Fixed signature of `getAppUserDataDir`.

## Path IO 0.2.0

* Added functions from `temporary`: `withTempFile`, `withTempDir`,
  `withSystemTempFile`, `withSystemTempDir`, `openTempFile`,
  `openBinaryTempFile`, and `createTempDir`. `temporary` is a lightweight
  and ubiquitous package, so depending on it should be OK.

## Path IO 0.1.1

* Fixed type signatures of `renameFile` and `copyFile`.

## Path IO 0.1.0

* Initial release.
