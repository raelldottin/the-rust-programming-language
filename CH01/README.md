# The Rust Programming Language
# Steve Klabnik, Carol Nichols, Contributions from the Rust Community
# This material may be protected by copyright. The Rust Programming Language

## Rust Installation
```console
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh

```
The rustup command can used to install and manage rust installations.
The curl command sownloads a script and the sh command runs the script which installs the rustup tool and rust.


```console
$ xcode-select --install
```
On macos, install the C compiler by installing xcode command line tools.


## Rust Troubleshooting
```console
$ rustc --version
rustc x.y.z (abcabcabc yyyy-mm-dd
```
The rustc command will display the version number if Rust is installed correctly.

## Rust Updating
```console
$ rustup update
```
This command will update Rust if it was installed via rustup.

## Rust Uninstalling
```console
$ rustup self uninstall
```
This command will uninstall Rust and the rustup script

## Rust Local Documentation
```console
$ rustup doc
```
This command will open the local documentation in your web browser.

## Anatomy of a Rust Program

```rust
fn main() {
    println!("Hello, world!");
}
```

In Rust, the main function is the first code that runs in a Rust program.
If the function has parameters, it would be placed inside the parentheses.
The body of the main function holds code that is executed.
Rust uses 4 spaces and not a tab for indents.
If a function ends with a !, its a marco and not function.
The end of a code line has a ;.

```console
$ rustfmt
```
The rustfmt command is an automatic formatter tool included in the standard Rust distribution.


```console
$ rustc main.rs
```
The rustc command creates a binary executable from your source code.

## Rust's build system and package manager is called Cargo
```console
$ cargo --version
```
The cargo command is installed with Rust and you can use command above to verify that it's installed.

## Creating a Project with Cargo
``` console
$ cargo new hello_cargo
$ cd hello_cargo
```


The project folder consists of:
- Cargo.toml file
- src directory
..- main.rs file inside


```toml
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2021"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
```
The TOML filr is cargo's configuration file.

```console
$ cargo build
```
This command produces an executable file.


```console
$ cargo run
```
This command runs the executable file.

```console
$ cargo check
```
This will check your code for compile errors and doesn't produce an executable.


```console
$ cargo build --release
```
This will build your executable with optimizations.
