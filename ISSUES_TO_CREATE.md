# ISSUES TO CREATE — High-level TODOs found

This file was generated automatically to capture and prioritize TODO/FIXME comments discovered in the repository. Create GitHub issues from the entries below and assign labels like `area:build`, `area:tooling`, `priority:low/med/high` as appropriate.

---

1. File: `tensorflow/tools/toolchains/win2022/BUILD`
   - TODO: `TODO(b/457398048): Deprecate the above platform once this one is working.`
   - Suggested issue: "Deprecate legacy Windows toolchain platform" — label: `area:build`, `priority:low`

2. File: `tensorflow/tools/toolchains/remote_config/rbe_config.bzl`
   - TODO: `TODO(b/369382309): Remove this once ml_build_rbe_config is used everywhere.`
   - Suggested issue: "Remove legacy RBE config after migration" — label: `area:build`, `priority:med`

3. File: `tensorflow/workspace2.bzl`
   - TODO: `Remove def file filter when TensorFlow can export symbols properly on Windows.`
   - Suggested issue: "Investigate Windows symbol export and remove def file filter" — label: `area:windows`, `priority:med`

4. File: `tensorflow/tools/toolchains/cross_compile/cc/cc_toolchain_config.bzl`
   - TODO: `TODO(#8303): Mac crosstool should also declare every feature.`
   - Suggested issue: "Ensure macOS crosstool declares all features" — label: `area:build`, `priority:low`

5. File: `tensorflow/tools/tf_sig_build_dockerfiles/setup.cuda.sh`
   - TODO: `Review this file` — Suggested issue: "Review CUDA-enabled Dockerfile setup scripts" — label: `area:docker`, `priority:low`

6. File: `tensorflow/tools/tf_sig_build_dockerfiles/devel.requirements.txt`
   - TODO about supporting older NumPy for TFX — label: `area:deps`, `priority:med`

7. File: `tensorflow/tools/proto_text/gen_proto_text_functions_lib_test.cc`
   - TODO to re-enable a test after float precision fix — label: `area:tests`, `priority:med`

8. File: `tensorflow/tools/proto_splitter/chunk.proto`
   - TODO to add sfixed key types if needed — label: `area:proto`, `priority:low`

9. Files in `tools/toolchains/clang6` and other toolchain templates with TODOs to clean up options and features — label: `area:build`, `priority:low`

---

Notes and suggested next steps:
- Review TODOs and convert each into an issue with reproduction steps or a short plan.
- Triage and prioritize items that affect builds, security, and CI first.
- Add an automated check (CI job) for new TODOs or for TODO age to avoid technical debt growth.

If you'd like, I can:
- Create the GitHub issues automatically (requires your permission and repository access token), or
- Open a draft PR with fixes for low-risk TODOs (I can start with the logging changes already applied), or
- Continue by running `ruff` and `mypy` on `tensorflow/lite` and prepare a list of actionable fixes.
