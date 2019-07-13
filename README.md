# nerData
ner语料优化
本文主要是针对https://github.com/Determined22/zh-NER-TF 这个开源工程中的一个ner语料进行优化
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713160539878.png)
非常标准的命名实体识别语料，语料的质量也是非常的高。
但是有个小问题
语料对于人物的标注，有非常多带称谓的人物只标注的姓
导致识别到非常多单字的姓效果非常差。
例如张女士、和张师傅识别结果都是张、张。
但我认为称谓也应该附带上
这边我花了两天时间，对语料中大约八百处标注进行了修改
**原始语料**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713161049453.png)![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713161014712.png)
**修改之后**
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713161034166.png)
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713161059260.png)
**识别结果对比**
语料修改之前的识别效果
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019071316162612.png)

修改之后的重新训练的识别结果
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190713161734404.png)
可以看到效果非常的显著

最后非常感谢大佬开源的工程，现也将语料公开
[csdn下载链接](https://download.csdn.net/download/cyz52/11343606)

