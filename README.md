# Java
Java自学啊啊啊啊啊啊

大概是从10月28号前开始撸视频的，今天看到150，集合，前面的由于太多乱七八糟的有点记不住了。

11/4
Collection的常用方法 Collectio c = new Collection();
                    c.add(Object o);向集合中添加元素。
                    c.size()返回int 集合中有几个元素。
                    c.contains(Object o);返回布尔型值，底层调用的是equals方法，判断集合中是否包含某元素。
                    存储在集合中的元素应该重写equals方法。
                    c.remove(Object o); 返回布尔型，底层调用的也是equals方法，删除集合中某元素。
                 迭代器的remove与集合自带的remove
                    Iterator it = new c.iterator();
                    While(it.next()){
                    it.next();
                    it.remove();}
                    如果用集合自身带的remove删除元素 会改变迭代器，推荐用迭代器删除。
List集合存储元素特点：1.有序 （存进去是这个顺序，取出来还是按照这个顺序取出）
                    2.可重复
                 List 是 Collection 的一个子接口继承Collection方法。
                 List中有一个get(int index)方法，collection中没有。
                 可以 List l=new ArrayList();(多态）
     Arraylist底层是数组，有下标，默认初始化容量是10，扩大之后的容量是原容量的1.5倍
     Vector底层是数组,默认初始化容量是10，扩大之后的容量是原容量的2倍
     推荐创建集合的时候指定初始化容量。
     可以通过下标来取元素，l.get(0);取集合第一个元素，
     遍历：for(int i=0;i<l.size();i++){
              Object o= l.get(i);
              System.out.println(o);
           } 
Set 集合存储元素特点:1.无序
                    2.不可重复
                 Set 是 Collection 的一个子接口继承Collection方法。
     HashSet底层实际上是一个HashMap，HashMap底层是哈希表/散列表。
          哈希表是，数组和单向链表的结合，哈希表本质是一个数组，只不过这个数组中的每一个元素又是一个单向链表（类似于字典）
          每一个单向链表都有一个哈希值代表数组下标，在某个单向链表中的每一个节点上是hash值都是相等的
          HashSet其实就是HashMap中的key部分，HashMap中的key有什么特点，HashMap中的key应该具有相同的特点。
          HashMap和HashSet初始化容量都是16，默认加载因子是0.75（当存储到容量的75%时自动扩容）
     关于往Set集合中存储的元素的HashCode和equals方法.存储在HashSet或者HashMap集合key部分的元素，需要重写hashCode和equals方法
     SortedSet无序不可重复，并按照顺序排列，被存储的元素需要重写compareto方法
 Map的常用的方法:clear（）;清空Map
                containsKey(Object key)判断Map中是否包含这样的key
                containsValue(Object vaule)判断Map中是否包含这样的value
                .....不想写了....
                remove（Object key）;通过key删除键值对
  Map中key重复了value采用覆盖的形式;
                
          
          
          
          
          
          
          

