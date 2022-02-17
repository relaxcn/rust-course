# 多线程并发编程
安全和高效的处理并发是 Rust 语言的主要目标之一。随着现代处理器的核心数不断增加，并发和并行已经成为日常编程不可或缺的一部分，甚至于 Go 语言已经将并发简化到一个 `go` 关键字就可以。

可惜的是，在 Rust 中由于语言设计理念、安全、性能的多方面考虑，并没有采用 Go 语言大道至简的方式，而是选择了多线程与 `async/await` 相结合，优点是可控性更强、性能更高，缺点是复杂度并不低，当然这也是系统级语言的应有选择：**使用复杂度换取可控性和性能**。

不过，大家也不用担心，本书的目标就是降低 Rust 使用门槛，这个门槛自然也包括如何在 Rust 中进行异步并发编程，我们将从多线程以及 async/await两个方面去深入浅出地讲解，首先，从本章的多线程开始。

在本章，我们将深入讲解并发和并行的区别以及如何使用多线程进行 Rust 并发编程，那么先来看看何为并行与并发。