# Summary

[简介](index.md)

- [Hello World](hello.md)
  - [注释](hello/comment.md)
  - [格式化输出](hello/print.md)
    - [调试（debug）](hello/print/print_debug.md)
    - [显示（display）](hello/print/print_display.md)
    - [测试实例：List](hello/print/print_display/testcase_list.md)
    - [格式化](hello/print/fmt.md)

- [原生类型](primitives.md)
  - [字面量和运算符](primitives/literals.md)
  - [元组](primitives/tuples.md)
  - [数组和切片](primitives/array.md)

- [自定义类型](custom_types.md)
  - [结构体](custom_types/structs.md)
  - [枚举](custom_types/enum.md)
    - [使用 use](custom_types/enum/enum_use.md)
    - [C 风格用法](custom_types/enum/c_like.md)
    - [测试实例：链表](custom_types/enum/testcase_linked_list.md)
  - [常量](custom_types/constants.md)

- [变量绑定](variable_bindings.md)
  - [可变变量](variable_bindings/mut.md)
  - [作用域和遮蔽](variable_bindings/scope.md)
  - [变量先声明](variable_bindings/declare.md)
  - [冻结](variable_bindings/freeze.md)

- [类型系统](types.md)
  - [类型转换](types/cast.md)
  - [字面量](types/literals.md)
  - [类型推断](types/inference.md)
  - [别名](types/alias.md)

- [类型转换](conversion.md)
  - [`From` 和 `Into`](conversion/from_into.md)
  - [`TryFrom` 和 `TryInto`](conversion/try_from_try_into.md)
  - [`ToString` 和 `FromStr`](conversion/string.md)

- [表达式](expression.md)

- [流程控制](flow_control.md)
  - [if/else](flow_control/if_else.md)
  - [loop 循环](flow_control/loop.md)
    - [嵌套循环和标签](flow_control/loop/nested.md)
    - [从 loop 循环返回](flow_control/loop/return.md)
  - [while 循环](flow_control/while.md)
  - [for 循环和区间](flow_control/for.md)
  - [match 匹配](flow_control/match.md)
    - [解构](flow_control/match/destructuring.md)
      - [元组](flow_control/match/destructuring/destructure_tuple.md)
      - [枚举](flow_control/match/destructuring/destructure_enum.md)
      - [指针和引用](flow_control/match/destructuring/destructure_pointers.md)
      - [结构体](flow_control/match/destructuring/destructure_structures.md)
    - [卫语句](flow_control/match/guard.md)
    - [绑定](flow_control/match/binding.md)
  - [if let](flow_control/if_let.md)
  - [while let](flow_control/while_let.md)

- [函数](fn.md)
  - [方法](fn/methods.md)
  - [闭包](fn/closures.md)
    - [捕获](fn/closures/capture.md)
    - [作为输入参数](fn/closures/input_parameters.md)
    - [类型匿名](fn/closures/anonymity.md)
    - [输入函数](fn/closures/input_functions.md)
    - [作为输出参数](fn/closures/output_parameters.md)
    - [`std` 中的例子](fn/closures/closure_examples.md)
      - [Iterator::any](fn/closures/closure_examples/iter_any.md)
      - [Iterator::find](fn/closures/closure_examples/iter_find.md)
  - [高阶函数](fn/hof.md)
  - [发散函数](fn/diverging.md)

- [模块](mod.md)
  - [可见性](mod/visibility.md)
  - [结构体的可见性](mod/struct_visibility.md)
  - [`use` 声明](mod/use.md)
  - [`super` 和 `self`](mod/super.md)
  - [文件分层](mod/split.md)

- [crate](crates.md)
  - [库](crates/lib.md)
  - [使用库](crates/using_lib.md)

- [cargo](cargo.md)
  - [依赖](cargo/deps.md)
  - [约定规范](cargo/conventions.md)
  - [测试](cargo/test.md)
  - [构建脚本](cargo/build_scripts.md)

- [属性](attribute.md)
  - [死代码 `dead_code`](attribute/unused.md)
  - [`crate`](attribute/crate.md)
  - [`cfg`](attribute/cfg.md)
    - [自定义条件](attribute/cfg/custom.md)

- [泛型](generics.md)
  - [函数](generics/gen_fn.md)
  - [实现](generics/impl.md)
  - [trait](generics/gen_trait.md)
  - [约束](generics/bounds.md)
    - [测试实例：空约束](generics/bounds/testcase_empty.md)
  - [多重约束](generics/multi_bounds.md)
  - [where 子句](generics/where.md)
  - [`newtype` 惯用法](generics/new_types.md)
  - [关联项](generics/assoc_items.md)
    - [存在问题](generics/assoc_items/the_problem.md)
    - [关联类型](generics/assoc_items/types.md)
  - [虚类型参数](generics/phantom.md)
    - [测试实例：单位检查](generics/phantom/testcase_units.md)

- [作用域规则](scope.md)
  - [RAII](scope/raii.md)
  - [所有权和移动](scope/move.md)
    - [可变性](scope/move/mut.md)
    - [部分移动](scope/move/partial_move.md)
  - [借用](scope/borrow.md)
    - [可变性](scope/borrow/mut.md)
    - [别名使用](scope/borrow/alias.md)
    - [ref 模式](scope/borrow/ref.md)
  - [生命周期](scope/lifetime.md)
    - [显式标注](scope/lifetime/explicit.md)
    - [函数](scope/lifetime/fn.md)
    - [方法](scope/lifetime/methods.md)
    - [结构体](scope/lifetime/struct.md)
    - [trait](scope/lifetime/trait.md)
    - [约束](scope/lifetime/lifetime_bounds.md)
    - [强制转换](scope/lifetime/lifetime_coercion.md)
    - [static](scope/lifetime/static_lifetime.md)
    - [省略](scope/lifetime/elision.md)

- [特质 trait](trait.md)
  - [派生](trait/derive.md)
  - [使用 `dyn` 返回 trait](trait/dyn.md)
  - [运算符重载](trait/ops.md)
  - [Drop](trait/drop.md)
  - [Iterator](trait/iter.md)
  - [`impl Trait`](trait/impl_trait.md)
  - [Clone](trait/clone.md)
  - [父 trait](trait/supertraits.md)
  - [消除重叠 trait](trait/disambiguating.md)

- [使用 `macro_rules!` 来创建宏](macros.md)
  - [语法](macros/syntax.md)
    - [指示符](macros/designators.md)
    - [重载](macros/overload.md)
    - [重复](macros/repeat.md)
  - [DRY (不写重复代码)](macros/dry.md)
  - [DSL (领域专用语言)](macros/dsl.md)
  - [可变参数接口](macros/variadics.md)

- [错误处理](error.md)
  - [`panic`](error/panic.md)
  - [`Option` 和 `unwrap`](error/option_unwrap.md)
    - [使用 `?` 解开 `Option`](error/option_unwrap/question_mark.md)
    - [组合算子：`map`](error/option_unwrap/map.md)
    - [组合算子：`and_then`](error/option_unwrap/and_then.md)
  - [结果 `Result`](error/result.md)
    - [`Result` 的 `map`](error/result/result_map.md)
    - [给 `Result` 取别名](error/result/result_alias.md)
    - [提前返回](error/result/early_returns.md)
    - [引入 `?`](error/result/enter_question_mark.md)
  - [处理多种错误类型](error/multiple_error_types.md)
    - [从 `Option` 中取出 `Result`](error/multiple_error_types/option_result.md)
    - [定义一种错误类型](error/multiple_error_types/define_error_type.md)
    - [把错误 “装箱”](error/multiple_error_types/boxing_errors.md)
    - [`?` 的其他用法](error/multiple_error_types/reenter_question_mark.md)
    - [包裹错误](error/multiple_error_types/wrap_error.md)
  - [遍历 `Result`](error/iter_result.md)

- [标准库类型](std.md)
  - [箱子、栈和堆](std/box.md)
  - [动态数组 vector](std/vec.md)
  - [字符串 String](std/str.md)
  - [选项 `Option`](std/option.md)
  - [结果 `Result`](std/result.md)
    - [`?` 用法](std/result/question_mark.md)
  - [`panic!`](std/panic.md)
  - [散列表 HashMap](std/hash.md)
    - [更改或自定义关键字类型](std/hash/alt_key_types.md)
    - [散列集 HashSet](std/hash/hashset.md)
  - [RC计数引用 Rc](std/rc.md)
  - [ARC共享计数引用 Arc](std/arc.md)

- [标准库更多介绍](std_misc.md)
  - [线程](std_misc/threads.md)
    - [测试实例：map-reduce](std_misc/threads/testcase_mapreduce.md)
  - [通道](std_misc/channels.md)
  - [路径](std_misc/path.md)
  - [文件输入输出（I/O）](std_misc/file.md)
    - [打开文件 `open`](std_misc/file/open.md)
    - [创建文件 `create`](std_misc/file/create.md)
    - [读取行 `read lines`](std_misc/file/read_lines.md)
  - [子进程](std_misc/process.md)
    - [管道](std_misc/process/pipe.md)
    - [等待](std_misc/process/wait.md)
  - [文件系统操作](std_misc/fs.md)
  - [程序参数](std_misc/arg.md)
    - [参数解析](std_misc/arg/matching.md)
  - [外部语言函数接口](std_misc/ffi.md)

- [测试](testing.md)
  - [单元测试](testing/unit_testing.md)
  - [文档测试](testing/doc_testing.md)
  - [集成测试](testing/integration_testing.md)
  - [开发依赖](testing/dev_dependencies.md)

- [不安全操作](unsafe.md)

- [兼容性](compatibility.md)
  - [原始标志符](compatibility/raw_identifiers.md)

- [补充](meta.md)
  - [文档](meta/doc.md)
  - [Playpen](meta/playpen.md)
