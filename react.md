# 一个JavaScript的搭建视图的库  采用声明式：只需要声明  不需要亲自操作dom  
    1.组件化：一个页面上一部分 所需要的所有的资源的集合叫做一个组件
    2.react native 可以开发安卓和iOS
    3.高效 DOM的diff算法  编码人员不直接操作DOM 最小化重绘
# 组件实例有三大属性
    1.state：
        1.值是对象；
        2.组件被称为状态机，通过更改组件的state改变页面的渲染
    2.props:参数
        1.
    3.ref
# 生命周期函数 === 生命周期钩子
    1.挂载
    2.更新
    3.卸载
# Diff算法：
    1.每次更新的时候 会重新调用render 渲染出来新的与旧的虚拟DOM树对比 进行部分结构的重绘或重排  最小单位是标签
    虚拟DOM的key是实现Diff算法的关键  
    key是虚拟DOM对象的标识
    在更新的时
    找到key相同的旧的DOM 若新的DOM没变则使用旧的虚拟DOM不去刷新页面 若是变了就用新的虚拟DOM刷新页面
    旧的虚拟DOM没能找到相同的KEY则创建新的虚拟DOM渲染到真实的页面上去