
### intellij idea 的设置和 key map里面有方块乱码,请问是什么问题?


Appearance->override default font 
Name: Dialog.plain
设置这个，idea的菜单字体

我是appearance 使用Dialog.plain字体， editor下的colors&Fonts使用的是Meslo字体
editor->appearance->use anti-aliased font 勾上

在 IntelliJ Idea 上设置 ：
Appearance->override default font 
Name: Dialog 
也可以解决

### IntelliJ IDEA，代码行宽度超出限制时自动换行

在File->settings->Code Style->General中，修改“Right margin (columns)”的值即可改变代码行宽度的限制。

有人会问，如果输入的代码超出宽度界线时，如何让IDE自动将代码换行？有两种方式！第一种，在上述的“Right margin (columns)”的下方，有“Wrap when typing reaches right margin”选项，选中它，是什么效果呢？如下图所示，随着输入的字符的增加，当代码宽度到达界线时，IDEA会自动将代码换行。

第一种方式是在输入代码时触发，还有第二种方式，在File->settings->Code Style->Java中，选中“Wrapping and Braces”选项卡，在“Keep when reformatting”中有一个“Ensure rigth margin is not exceeded”，选中它，是什么效果呢？从配置项的字面意思很容易理解，在格式化Java代码时，确保代码没有超过宽度界线。

不要紧，按下“Ctrl+Alt+L”格式化代码。 


IDE能帮我们在超出代码宽度界线时自动换行自然是好，可上述两种方式依旧有不妥之处，就是IDE只会帮我们主动换行一次！当IDE自动换行后，代码长度依旧超出界线时，就需要手动处理了。而且不难看出IDE所做的换行处理简单粗暴，未必是我们想要的结果（有时我们期望可以字符串换行拼接可能更优雅些）。

所以我个人建议，IDE所给出的宽度界线是好的，但真正控制、优化代码宽度的格式需要我们编码时养成良好的习惯，避免单行代码过长，避免不了时自己手动找到合适的截点，进行换行处理，且更符合各自实际的编码格式需求。
