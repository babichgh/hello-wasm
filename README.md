# hello-wasm
## Prerequisites
- [rustup](https://rust-lang.org/tools/install/)
- Python
## Installation
1. Clone the repository:
   ```
   git clone https://github.com/babichgh/hello-wasm.git
   cd hello-wasm
   ```
2. Install wasm-pack
   ```
   cargo install wasm-pack
   ```
3. Build
   ```
   wasm-pack build --target web
   ```
4. Start a simple http server
   ```
   python -m http.server 8080
   ```
5. Open http://localhost:8080 in your browser. You'll see **Hello, WASM!**
## Project structure
```
file-writer/
├── srs/
    └── lib.rs   # Rust source code
├── .gitignore   # Ignores /target
├── Cargo.lock   # Helps compile
├── Cargo.toml   # Dependencies are here
├── README.md    # You read it right now
└── index.html   # HTML file
```
