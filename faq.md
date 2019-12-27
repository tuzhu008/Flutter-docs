## StatefulWidget 和 State 为啥是分开的对象？

在 Flutter 中，这两种类型的对象具有不同的生命周期。`Widgets`是临时对象，用于在当前状态下构造应用程序的表示形式。另一方面，`State` 对象在两次 `build()` 调用之间保持不变，从而使它能记住这些信息。

