# hilbert_transform_rs

Hilbert_transform is a library written in Rust to perform the hilbert transformation like Matlab/Octave or scipy.signals.hilbert.

Hilbert_transform is implemented based on scipy implementation of same function.

# Usage

```rust
use hilbert_transform::{hilbert};

fn main() {
    let input = vec![1.0, 2.0, 3.0, 4.0];     
    let hilbert_output = hilbert(&input);
    println!("{:?}", hilbert_output);
    // hilbert_output will be equal to: [Complex { re: 1.0, im: 1.0 }, Complex { re: 2.0, im: -1.0 }, Complex { re: 3.0, im: -1.0 }, Complex { re: 4.0, im: 1.0 }]
}
```
