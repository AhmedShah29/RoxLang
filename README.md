# RoxLang
A high level programming language with full control and customizability 
> note this is still a design check the [wiki](https://github.com/AhmedShah29/RoxLang/wiki) for the last updates.
### simple flowchart
```mermaid
graph TD
    rox["Rox"]
    rox --> compiler["Compiler — rcc"]
    rox --> vm["VM/Interpreter"]
    rox --> rkm["rkm — package manager"]
    rox --> tracker["Memory Tracker"]

    compiler --> native["Native binary via (Clang/LLVM)"]
    vm --> bytecode["Bytecode + optional JIT"]
    rkm --> git["Clone/push libs via GitHub"]
    tracker --> log["Memory usage log"]
```
