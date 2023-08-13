## Note: Even though this version retains all the logic from the original repository, always adhere to the "zero trust" principle and use this release at your own risk. We are *not* responsible for any malfunctions and potential damage. However, we guarantee on our part that this version preserves 100% of the original code, except for the adjustment of the fee from 1000 to 10000 zat.

 You have the flexibility to adjust the transaction fee as per your needs. To do this:

Clone the following three repositories into a single directory: [zecwallet-lite](https://github.com/kattywood/zecwallet-lite), [zecwallet-light-cli](https://github.com/kattywood/zecwallet-light-cli), and [librustzcash](https://github.com/kattywood/librustzcash).

Navigate to librustzcash\zcash_primitives\src\transaction\components\amount.rs and on line 10, modify the value from "10000" to your preferred amount in the line
* pub const DEFAULT_FEE: Amount = Amount(10000).

Once the changes are made, you can then compile the project using the source code.
	
 # Zcash Rust crates

This repository contains a (work-in-progress) set of Rust crates for
working with Zcash.

## Security Warnings

These libraries are currently under development and have not been fully-reviewed.

## License

All code in this workspace is licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

Downstream code forks should note that some (but not all) of these crates
and components depend on the 'orchard' crate, which is licensed under the
[Bootstrap Open Source License](https://github.com/zcash/orchard/blob/main/LICENSE-BOSL).
A license exception is provided allowing some derived works that are linked or
combined with the 'orchard' crate to be copied or distributed under the original
licenses (in this case MIT / Apache 2.0), provided that the included portions of
the 'orchard' code remain subject to BOSL.
See <https://github.com/zcash/orchard/blob/main/COPYING> for details of which
derived works can make use of this exception, and the `README.md` files in
subdirectories for which crates and components this applies to.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.
