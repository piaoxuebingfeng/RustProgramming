# 安装与使用 rustc



## Rust 安装

  rust 官方安装说明网站。

  https://www.rust-lang.org/tools/install

### Linux Ubuntu

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs |sh
```

  检查是否安装成功。

  安装完成之后，重新启动一个终端，运行以下指令，检查是否能够运行成功。

```bash
rustc --version

cargo --version
```



## Hello World



```rust
// 这是一行注释

//主函数
fn main(){
    // 将文本打印到控制台
    println!("Hello World!");
}
```

  `println!` 是一个宏，用于将文本输出到控制台(console).



  编译 `rustc`

```bash
rustc hello.rs
```

  运行 `hello`

```bash
./hello
```



## rust 语言注释

  Rust 支持几种不同风格的注释方式。



- 普通注释
  - // 单行注释，注释内容直到行尾
  - /*  块注释，注释内容一直到结束分隔符。 */

- 文档注释
  - /// 为接下来的项生成帮助文档
  - //! 为注释所属于的项 生成帮助文档

  文档注释是一种特殊的注释方式，用于生成 html 文档。

  如果是使用 cargo 构建的 rust 项目，可以使用 cargo 命令来生成文档。

```bash
# 生成文档并在浏览器中打开
cargo doc --open

# 生成文档
cargo doc
```



## cargo 基本使用



```bash
# 创建一个 helloworld 的 rust 项目
cargo new helloworld

cd helloworld

# 构建项目
cargo build

# 运行项目
cargo run

# 生成文档
cargo doc
```





