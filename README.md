ZLUDA is a drop-in replacement for CUDA on non-NVIDIA GPUs. ZLUDA allows running unmodified CUDA applications using non-NVIDIA GPUs with near-native performance

<div align="center">

<!-- 80x28 104.75x28  62x28-->
[<img src="https://img.shields.io/badge/quick start-green?style=for-the-badge&logo=readthedocs&logoColor=white" width="267.5" height="56">](https://zluda.readthedocs.io) [<img src="https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white" width="209.5" height="56">](https://discord.gg/sg6BNzXuc7) [<img src="https://img.shields.io/badge/news-red?style=for-the-badge&logo=book&logoColor=white" width="124" height="56">](https://vosen.github.io/ZLUDA/)

<div/>

## CI

The [`.github/workflows/ci.yml`](.github/workflows/ci.yml) workflow runs on every pull request and on pushes to `master`. It checks whitespace and Rust formatting, and runs `cargo clippy` (warnings as errors), `cargo check` and `cargo build` on the crates that do not depend on the ROCm/HIP runtime or the `ext/llvm-project` and `ext/HiGHS` submodules. GPU builds and on-device tests are covered by the separate `pr_master` and `push_master` workflows.
