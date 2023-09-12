# Chapter 1
# Rust installation
For installing and managing Rust toolchain we will need rustup.
for installing rustup you could go to https://www.rust-lang.org/tools/install and select the installation method for your os
### Linux
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
### Windows
Are you really, really sure to install it on windows?
You could download and run [rustup-init.exe](https://static.rust-lang.org/rustup/dist/i686-pc-windows-gnu/rustup-init.exe)

## Using rustup
For installing stable rust you could follow the installation guide, or you could run:
```bash
rustup toolchain instal stable
```
Now we have rust installed, it could be neccessary to reload the shell or add the directory to PATH enviroment variable

## First project
For creating a new project we will use cargo to manage all the dependencies and configuration.
Simply we execute:
 ```bash
cargo new <NAME_OF_PROJECT>
```
The structure of the project should be:

```bash
<NAME_OF_PROJECT>
├── Cargo.toml
└── src
    └── main.rs
``` 
Where:
- Cargo.toml: contains all the cargo magic with dependencies, various metadata if you will ever publish your crate and so on.
- src: all our source code should be inside this folder
- main.rs the root of our project, write your rust code in there.

In the end we need to execute our code with this comand.
```ssh
cargo run 
```
For more information, you could read from the excellent [rust book](https://doc.rust-lang.org/book/ch01-00-getting-started.html).
