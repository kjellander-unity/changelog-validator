# Changelog validator
Command line tool for validating `CHANGLELOG.md` similar to ump-ci does it.

# Goal
To have a quick way to run the `ump-ci` validation on `CHANGLELOG.md` in isolation, so it can be run independently for small commits that only change the `CHANGELOG.md`. 

# Implementation details

Since https://github.cds.internal.unity3d.com/unity/com.unity.package-validation-suite/blob/master/Editor/ValidationSuite/ValidationTests/ChangeLogValidation.cs is what we want to run, but it's an `internal` class, we have to clone the source. This is done using `git submodules`.

# References

* https://github.cds.internal.unity3d.com/unity/upm-ci-utils - home of `ump-ci`, which in turn uses this for the validation:
* https://github.cds.internal.unity3d.com/unity/com.unity.package-validation-suite/blob/master/Editor/ValidationSuite/ValidationTests/ChangeLogValidation.cs
