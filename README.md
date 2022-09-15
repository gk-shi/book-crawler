### 图书分享脚本



> 注意：因为代码最后是上传到我个人服务器，所以想了解过程的话，实践前请先修改代码最后上传服务器地址，感谢！
>
> 
>
> ⚠️项目代码仅供学习！⚠️



#### 1. 是什么

一个油猴脚本，用来抓取自己的掘金小册内容并分享。

#### 2.目前适用范围

- 掘金小册

#### 3. 使用方法

- step1

  安装油猴脚本

- step2

   通过链接[图书分享](https://greasyfork.org/zh-CN/scripts/450389-%E5%9B%BE%E4%B9%A6%E5%88%86%E4%BA%AB)访问脚本下载安装(由于非公开发布脚本，只能通过链接访问)

- step3

  首先需要进入到小册内容的非第一章节(虽然做了额外处理，但这样会减少不确定性)，然后⚠️**刷新页面，等待页面所有接口加载完成（要标签栏没有小圆圈在转了，因为评论是另外的请求，它的响应会稍微慢一点）⚠️，之后会在标题旁边出现一个`开始复制`的按钮(⚠️请等文章、评论渲染完了在点击！因为加入了评论的抓取**⚠️)。

  ![image-20220314153547323](/readme_img/i5.png)

- step4

  点击按钮，然后程序会自动模拟章节的顺序点击，不用做额外的操作，在章节旁边会显示章节是否抓取成功。做了模拟延迟点击，限制是 2s ~ 3.5s 随机点击下一章获取内容，所以需要等等。

  ![image-20220314154157546](/readme_img/i6.png)

  最后会有弹窗确定是否上传到我的服务器成功。
  ![image-20220314154157546](/readme_img/i7.png)
