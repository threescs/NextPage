# NextPage
手写一个移动端的下拉分页


准备就绪 需求分析
滑动到屏幕底部,自动加载下一页数据

设计思路///
1.分析元素是否在可视区
2.获取发送请求的url
3.原生http请求 (加载成功调用function 失败调用 卸载function)
4.判断请求状态 (xhr readyState ! = 4)
5.遍历DOM查询是否符合加载条件
6.把需要监听的事件进行绑定 (load touchstart touchend click haschange scroll......)
