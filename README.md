# 以下是使用fuzzy_AHP时的一些注意事项：
1.	fuzzy_AHP是一个基于Python的、可以完成分权任务和利用DEAP2.1模型对供应商排名进行复核的应用程序，主要用于对供应商月度服务调查问卷的权重分配以及在EXCEL计算得到供应商排名后的复核。
2.	通过咨询工厂负责人员得到的重要程度等数据应该录入同文件夹的“AHP主观排序“EXCEL文件中，每一个EXCEL文件只能将数据录入第一个sheet，每一个sheet中只能存在一组待分权的数据。请严格按照以下格式录入数据：A1	不填入任何内容；A2、A3、A4等和B1、C1、D1等填入本组的待分权标签；其它格填写重要程度的数字表示（注意调整EXCEL单元格格式为”一位分数“）。注意目前fuzzy_AHP只能处理数目在2-10以内的标签集合，标签数目多于10个会报错，可以通过修改原代码增加可处理标签数。
3.	权重结果会被输出在同目录下的“权重“EXCEL文件中。注意，在使用应用程序时，”权重“文件应处于关闭状态，以确保结果数据的正确写入。

个人存档
