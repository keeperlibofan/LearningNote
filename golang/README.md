### struct
```golang
type CustomClaims struct {
	User *pb.User
	jwt.StandardClaims
}
```
`jwt.StandardClaims`本身有实现的接口会被继承到`CustomClaims`上

### container/heap

heap是常用的实现优先队列的方法。要创建一个优先队列，实现一个具有使用（负的）优先级作为比较的依据的Less方法的Heap接口，如此一来可用Push添加项目而用Pop取出队列最高优先级的项目

``` golang
type Interface interface {
    sort.Interface
    Push(x interface{}) // add x as element Len()
    Pop() interface{}   // remove and return element Len() - 1.
```

