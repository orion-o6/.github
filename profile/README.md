# Orion O6

Community firmware work for the **Radxa Orion O6** (CIX P1 "Sky1" SoC): patches, build and flash tooling, and documentation.

We build the CIX community BIOS from source, and a self-built image signed with the OEM key flashes and boots on real hardware. That makes BL31 (TF-A), BL32 (OP-TEE), and BL33 (UEFI) patchable. bootloader1 stays stock, verified by the Security Enclave against a fused key.

### Start here

- **[firmware](https://github.com/orion-o6/firmware)**: patches, tooling, and the knowledge behind the work, including the boot trust model.
- **[Issues](https://github.com/orion-o6/firmware/issues)**: the board's real problems, tracked and worked in the open. Hitting one? Open an issue with your firmware version and a serial log if you have one.

We never redistribute closed blobs or signed images. You build your own from the CIX source plus our patches. Flashing experimental firmware needs an SPI programmer to recover, so do not flash without one.
