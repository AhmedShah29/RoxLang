# RoxLang
A high level programming language with control and customizability 
> note this is still in design, check the [wiki](https://github.com/AhmedShah29/RoxLang/wiki) for the latest updates.

### Ecosystem & Architecture
```mermaid
flowchart TD
    rox{"RoxLang"}

    rox ==> compiler["Compiler — rcc"]
    rox ==> vm["VM / Interpreter"]
    rox ==> rkm["Package Manager — rkm"]
    rox ==> tracker["Memory Tracker"]
    rox ==> fmt["Formatter — rfmt"]

    compiler -.-> native["Native binary (Clang/LLVM)"]
    vm -.-> bytecode["Bytecode runs on the VM"]
    rkm -.-> git["Clone/push libs via GitHub"]
    tracker -.-> log["Memory usage log"]
    fmt -.-> codestyle["Standardized code style"]
