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
     
     
     

