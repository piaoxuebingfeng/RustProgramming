# 安装与使用 rustc



## Rust 安装

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



