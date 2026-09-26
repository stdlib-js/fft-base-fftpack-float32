# CHANGELOG

> Package changelog.

<section class="release" id="unreleased">

## Unreleased (2026-09-26)

<section class="features">

### Features

-   [`8b79b91`](https://github.com/stdlib-js/stdlib/commit/8b79b919e9514ddaff25acddef991b4bbc16b8bd) - update `fft/base/fftpack/float32` TypeScript declarations [(#15551)](https://github.com/stdlib-js/stdlib/pull/15551)
-   [`cc80daa`](https://github.com/stdlib-js/stdlib/commit/cc80daa661dc09bfdfa0ac4eb9102a3ecdfb5582) - add `rfftf` to namespace
-   [`11f8bc3`](https://github.com/stdlib-js/stdlib/commit/11f8bc38811058795878ab3610a38a9c516abd0f) - add `fft/base/fftpack/float32/rfftf` [(#15379)](https://github.com/stdlib-js/stdlib/pull/15379)
-   [`0061913`](https://github.com/stdlib-js/stdlib/commit/0061913d2e65266d30537fb1548e1a7da6c73dfd) - update `fft/base/fftpack/float32` TypeScript declarations [(#15287)](https://github.com/stdlib-js/stdlib/pull/15287)
-   [`bbf5576`](https://github.com/stdlib-js/stdlib/commit/bbf55760716ee0e6d0eb5f74b4ac22390257475f) - update `fft/base/fftpack/float32` TypeScript declarations [(#15258)](https://github.com/stdlib-js/stdlib/pull/15258)
-   [`ed8ea0c`](https://github.com/stdlib-js/stdlib/commit/ed8ea0c7808eec0735fa06e3f9929531e21e8f82) - add `fft/base/fftpack/float32/sinqi` [(#14808)](https://github.com/stdlib-js/stdlib/pull/14808)
-   [`61956b3`](https://github.com/stdlib-js/stdlib/commit/61956b30de14ee2edb75722c3c8f9ed87dda9c9c) - add `fft/base/fftpack/float32/cosqi` [(#14786)](https://github.com/stdlib-js/stdlib/pull/14786)
-   [`13d01a9`](https://github.com/stdlib-js/stdlib/commit/13d01a960d64ecbf63628e52451b29cc27505eec) - update `fft/base/fftpack/float32` TypeScript declarations [(#14641)](https://github.com/stdlib-js/stdlib/pull/14641)
-   [`8654861`](https://github.com/stdlib-js/stdlib/commit/86548615a074f6e93475822200e291e95ca7761a) - add `rffti` to namespace
-   [`91248c1`](https://github.com/stdlib-js/stdlib/commit/91248c1ce18881e1be702dfc9788c0612c37a966) - add `fft/base/fftpack/float32/rffti` [(#14591)](https://github.com/stdlib-js/stdlib/pull/14591)
-   [`924fac8`](https://github.com/stdlib-js/stdlib/commit/924fac8e6b44b5df2482a709a0b8624f5d8682e5) - add `fft/base/fftpack/float32` namespace
-   [`5f8f798`](https://github.com/stdlib-js/stdlib/commit/5f8f798b9a8345f41975c6bcc7a580c58fd02f74) - add `fft/base/fftpack/float32/decompose` [(#14482)](https://github.com/stdlib-js/stdlib/pull/14482)

</section>

<!-- /.features -->

<section class="bug-fixes">

### Bug Fixes

-   [`be6f218`](https://github.com/stdlib-js/stdlib/commit/be6f2184b1659459908028947ab7404588e9a37d) - remove float32 emulation

</section>

<!-- /.bug-fixes -->

<section class="breaking-changes">

### BREAKING CHANGES

-   [`0061913`](https://github.com/stdlib-js/stdlib/commit/0061913d2e65266d30537fb1548e1a7da6c73dfd): write factors to workspace as Uint32Array view

    -   To migrate, workspace consumers should reinterpret the factors section as a `Uint32Array`. This enables support for longer sequence lengths.

-   [`bbf5576`](https://github.com/stdlib-js/stdlib/commit/bbf55760716ee0e6d0eb5f74b4ac22390257475f): write to a Uint32Array

    -   To migrate, consumers should provide a Uint32Array instead of a Float32Array. Doing so allows support for longer sequence lengths.

-   [`7333861`](https://github.com/stdlib-js/stdlib/commit/7333861bf0de5054a329c9941c92a46d716be4ce): reinterpret workspace array

    -   To migrate, consumers should reinterpret the factor section as a `Uint32Array` view, as demonstrated in documented examples.

-   [`a697555`](https://github.com/stdlib-js/stdlib/commit/a697555175a55d741bf5716b425a1b735b8de8c2): migrate from `Float32Array` to `Uint32Array`

    -   To migrate, users should replace providing a `Float32Array` with a `Uint32Array`. Doing so enables support for longer sequences.

</section>

<!-- /.breaking-changes -->

<section class="commits">

### Commits

<details>

-   [`8b79b91`](https://github.com/stdlib-js/stdlib/commit/8b79b919e9514ddaff25acddef991b4bbc16b8bd) - **feat:** update `fft/base/fftpack/float32` TypeScript declarations [(#15551)](https://github.com/stdlib-js/stdlib/pull/15551) _(by stdlib-bot)_
-   [`62cbbac`](https://github.com/stdlib-js/stdlib/commit/62cbbac0f25dddf13b832a1de15d11f2ddad03ca) - **docs:** fix description [(#15542)](https://github.com/stdlib-js/stdlib/pull/15542) _(by Gunj Joshi, Athan Reines)_
-   [`cc80daa`](https://github.com/stdlib-js/stdlib/commit/cc80daa661dc09bfdfa0ac4eb9102a3ecdfb5582) - **feat:** add `rfftf` to namespace _(by Athan Reines)_
-   [`11f8bc3`](https://github.com/stdlib-js/stdlib/commit/11f8bc38811058795878ab3610a38a9c516abd0f) - **feat:** add `fft/base/fftpack/float32/rfftf` [(#15379)](https://github.com/stdlib-js/stdlib/pull/15379) _(by Gunj Joshi, Athan Reines)_
-   [`0061913`](https://github.com/stdlib-js/stdlib/commit/0061913d2e65266d30537fb1548e1a7da6c73dfd) - **feat:** update `fft/base/fftpack/float32` TypeScript declarations [(#15287)](https://github.com/stdlib-js/stdlib/pull/15287) _(by stdlib-bot)_
-   [`625cd5d`](https://github.com/stdlib-js/stdlib/commit/625cd5d8f466e2e7312306a9d731634c9e77f4ce) - **docs:** update namespace table of contents [(#15288)](https://github.com/stdlib-js/stdlib/pull/15288) _(by stdlib-bot)_
-   [`bbf5576`](https://github.com/stdlib-js/stdlib/commit/bbf55760716ee0e6d0eb5f74b4ac22390257475f) - **feat:** update `fft/base/fftpack/float32` TypeScript declarations [(#15258)](https://github.com/stdlib-js/stdlib/pull/15258) _(by stdlib-bot)_
-   [`268814f`](https://github.com/stdlib-js/stdlib/commit/268814f8b0e017504112dd6e50e7836644273f6f) - **docs:** update namespace table of contents [(#15259)](https://github.com/stdlib-js/stdlib/pull/15259) _(by stdlib-bot)_
-   [`7333861`](https://github.com/stdlib-js/stdlib/commit/7333861bf0de5054a329c9941c92a46d716be4ce) - **refactor:** update `fft/base/fftpack/float32/rffti` to use integer array view [(#15247)](https://github.com/stdlib-js/stdlib/pull/15247) _(by Gunj Joshi, Athan Reines)_
-   [`7099552`](https://github.com/stdlib-js/stdlib/commit/7099552f0144bc0c4ab8aa5afc68796d14b469a6) - **docs:** remove duplicate lines [(#15246)](https://github.com/stdlib-js/stdlib/pull/15246) _(by Gunj Joshi)_
-   [`a697555`](https://github.com/stdlib-js/stdlib/commit/a697555175a55d741bf5716b425a1b735b8de8c2) - **refactor:** update `fft/base/fftpack/float32/decompose` to use integer array view [(#15224)](https://github.com/stdlib-js/stdlib/pull/15224) _(by Gunj Joshi, Athan Reines)_
-   [`ed8ea0c`](https://github.com/stdlib-js/stdlib/commit/ed8ea0c7808eec0735fa06e3f9929531e21e8f82) - **feat:** add `fft/base/fftpack/float32/sinqi` [(#14808)](https://github.com/stdlib-js/stdlib/pull/14808) _(by Gunj Joshi, Athan Reines)_
-   [`61956b3`](https://github.com/stdlib-js/stdlib/commit/61956b30de14ee2edb75722c3c8f9ed87dda9c9c) - **feat:** add `fft/base/fftpack/float32/cosqi` [(#14786)](https://github.com/stdlib-js/stdlib/pull/14786) _(by Gunj Joshi)_
-   [`13d01a9`](https://github.com/stdlib-js/stdlib/commit/13d01a960d64ecbf63628e52451b29cc27505eec) - **feat:** update `fft/base/fftpack/float32` TypeScript declarations [(#14641)](https://github.com/stdlib-js/stdlib/pull/14641) _(by stdlib-bot)_
-   [`436e791`](https://github.com/stdlib-js/stdlib/commit/436e791d013826eecbf13e2cf25a2037369fce10) - **docs:** update namespace table of contents [(#14643)](https://github.com/stdlib-js/stdlib/pull/14643) _(by stdlib-bot)_
-   [`8654861`](https://github.com/stdlib-js/stdlib/commit/86548615a074f6e93475822200e291e95ca7761a) - **feat:** add `rffti` to namespace _(by Athan Reines)_
-   [`91248c1`](https://github.com/stdlib-js/stdlib/commit/91248c1ce18881e1be702dfc9788c0612c37a966) - **feat:** add `fft/base/fftpack/float32/rffti` [(#14591)](https://github.com/stdlib-js/stdlib/pull/14591) _(by Gunj Joshi, Athan Reines)_
-   [`be6f218`](https://github.com/stdlib-js/stdlib/commit/be6f2184b1659459908028947ab7404588e9a37d) - **fix:** remove float32 emulation _(by Athan Reines)_
-   [`77d4d43`](https://github.com/stdlib-js/stdlib/commit/77d4d43ab30c6f6e6f18d2e712cc1865ded39cae) - **docs:** add JSDoc [(#14579)](https://github.com/stdlib-js/stdlib/pull/14579) _(by stdlib-bot)_
-   [`09f72aa`](https://github.com/stdlib-js/stdlib/commit/09f72aaa0ca90f3f4c9a7b6b9b8ad492e05ef7b9) - **docs:** update namespace table of contents [(#14584)](https://github.com/stdlib-js/stdlib/pull/14584) _(by stdlib-bot)_
-   [`924fac8`](https://github.com/stdlib-js/stdlib/commit/924fac8e6b44b5df2482a709a0b8624f5d8682e5) - **feat:** add `fft/base/fftpack/float32` namespace _(by Athan Reines)_
-   [`5f8f798`](https://github.com/stdlib-js/stdlib/commit/5f8f798b9a8345f41975c6bcc7a580c58fd02f74) - **feat:** add `fft/base/fftpack/float32/decompose` [(#14482)](https://github.com/stdlib-js/stdlib/pull/14482) _(by Gunj Joshi)_

</details>

</section>

<!-- /.commits -->

<section class="contributors">

### Contributors

A total of 2 people contributed to this release. Thank you to the following contributors:

-   Athan Reines
-   Gunj Joshi

</section>

<!-- /.contributors -->

</section>

<!-- /.release -->

