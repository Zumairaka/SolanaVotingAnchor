RUSTUP_TOOLCHAIN="nightly-2024-11-19" anchor build

or add
"[workspace.lints.rust.unexpected_cfgs]
level = "warn"
check-cfg = [
'cfg(target_os, values("solana"))',
]" to workspace cargo.toml
