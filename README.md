# backbone-study

任何时候只要UI事件引发起模型内的属性变化,模型会触发"change"事件,所有显示模型数据的View会接受到该通知,继而视图重新渲染.

Backbone试图定义一组最小而高效的集合,包括了数据结构(models,collections)和用户接口(views,urls).

backbone作为一个工具,让你可以随心所欲的设计你的网站.

##Backbone.Events(事件)

### on
object.on(event,callback,[context])  arial:bind

### off
object.off([event],[callback],[context]) arial:unbind

### trigger
object.trigger(event,[*args])

### once
once object.once(event,callback,[context])

###listenTo 
object.listenTo(other,event,callback)

###stopListening
object.stopListening([other],[event],[callback])

###listenToOnce 
object.listenToOnce(other,event,callback)

###事件目录

+ add
+ remove
+ reset
+ sort
+ change
+ change:[attribute]
+ destory
+ request
+ sync
+ error
+ invalid
+ route:[name]
+ route 
+ all

##Backbone.Model(模型)

###extend
Backbone.Model.extend(properties,[classProperties])

###constructor/initialize

new Model([attributes],[options])

attributes里的属性会被set到model,options参数可以包含collection和parse两个属性.
collection属性代表model属于的collection.如果{parse: true}被作为一个option选项传递， attributes将在 set到model之前首先通过parse被转换











