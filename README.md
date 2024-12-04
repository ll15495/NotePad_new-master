基本功能实现：
（一）笔记列表显示笔记条目的时间戳
1.在PROJECTION投影中添加NotePad.Notes.COLUMN_NAME_MODIFICATION_DATE

![img_1.png](img_1.png)

2.修改对应布局文件以显示时间戳

![img_2.png](img_2.png)

3.修改NoteList.java中对应字段

![img_3.png](img_3.png)

4.更改SimpleCursorAdapter中数据显示格式

![img_4.png](img_4.png)

5.完成时间戳显示功能

![img_5.png](img_5.png)

（二）笔记内容的搜索功能

1.在list_options_menu.xml中添加搜索框

![img_6.png](img_6.png)

2.重写onCreateOptionsMenu方法，加载菜单资源，并为搜索视图设置监听器。

![img_8.png](img_8.png)

3.使用搜索结果创建一个新的Cursor，然后更新ListView。

![img_9.png](img_9.png)

4.完成搜素功能

![img_10.png](img_10.png)
![img_11.png](img_11.png)
![img_12.png](img_12.png)

扩展功能实现：
（一）一键清空所有笔记功能
1.在 onCreateOptionsMenu 方法中添加一个新的菜单项

![img_13.png](img_13.png)

2.在 onOptionsItemSelected 方法中处理新的菜单项点击事件

![img_14.png](img_14.png)

3.实现clearAllNotes方法

![img_15.png](img_15.png)

4.一键清空所有笔记功能演示

![img_16.png](img_16.png)
![img_17.png](img_17.png)
![img_18.png](img_18.png)

（二）将笔记按首字母排序功能

1.在list_options_menu.xml中添加按首字母排序

![img_19.png](img_19.png)

2.在onOptionsItemSelected方法中处理新的排序菜单项

![img_20.png](img_20.png)

3.实现sortNotesByFirstLetter方法

![img_21.png](img_21.png)

4.将笔记按首字母排序功能演示

![img_22.png](img_22.png)
![img_23.png](img_23.png)
![img_24.png](img_24.png)