// {
//   // 使用 IntelliSense 了解相关属性。 
//   // 悬停以查看现有属性的描述。
//   // 欲了解更多信息，请访问: https://go.microsoft.com/fwlink/?linkid=830387
//   "version": "0.2.0",
//   "configurations": [
//     {
//       "name": "g++.exe - 生成和调试活动文件",
//       // type 告诉vscode编译器的类型，我用的MinGW64也就是g++，这里是cppdgb
//       // 这个是规定的，不是随便写，比如msvc编译器就是cppvsdbg
//       "type": "lldb",
//       "request": "launch", //有launch和attach可选，这里填launch，按下F5就可以启动调试了；而不是attach（附加）
//       // program 这个是你的可执行程序位置，这里可以根据自己的tasks.json生成
//       // 程序的位置自定义修改，等会参照后面的tasks.json内容
//       //程序所在路径和程序名
//       "program": "${fileDirname}\\${fileBasenameNoExtension}.exe",
//       //这里填命令行参数（main函数的形参）
//       // "args": [],
//       //为true时，在开始运行程序时，不立刻往后执行，先暂停一下，一般填false；
//       // "stopAtEntry": false,
//       //目标工作目录，在哪个目录调试程序，一般在当前文件夹（项目所在文件夹）；
//       "cwd": "${fileDirname}",
//       //临时手动添加环境变量；
//       // "environment": [],
//       //如果需要输入东西，最好修改为true使用外部控制台（在运行时额外打开终端）。否则用vscode内置的控制台不能输入东西（不是内联控制台，内联控制台和外部控制台其实是一样的，但是这里调试的时候没有内联控制台这个选项）
//       // "externalConsole": false,
//       //指定调试器gdb或lldb
//       // "MIMode": "lldb",
//       //调试器的路径
//       // "miDebuggerPath": "lldb",
//       // "setupCommands": [
//       //   {
//       //     "description": "为 gdb 启用整齐打印",
//       //     "text": "-enable-pretty-printing",
//       //     "ignoreFailures": true
//       //   }
//       // ],
//       //这个表示 执行调试前 要完成的任务 该值需要与tasks.json中的label相同，否则调试时会提示找不到；
//       "preLaunchTask": "C/C++: g++.exe 生成活动文件"
//     }
//   ]
// }