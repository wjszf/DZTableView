##视图控制器的作用

运行在iPhone OS上的应用程序在如何组织内容和如何将内容呈现给用户方面有很多选择。含有很多内容的应用程序可以将内容分为多个屏幕。在运行时，每个屏幕的背后都是一组视图对象，负责显示该屏幕的数据。一个屏幕的视图后面是一个视图控制器其作用是管理那些视图上显示的数据，并协调它们和应用程序其它部分的关系。

UIViewController类负责创建其管理的视图及在低内存时将它们从内容中移出。视图控制器还为某些标准的系统行为提供自动响应。比如，在响应设备方向变化时，如果应用程序支持该方向，视图控制器可以对其管理的视图进行尺寸调整，使其适应新的方向。您也可以通过视图控制器来将新的视图以模式框的方式显示在当前视图的上方。

除了基础的UIViewController类之外，UIKit还包含很多高级子类，用于处理平台共有的某些高级接口。特别需要提到的是，导航控制器用于显示多屏具有一定层次结构的内容；而页签条控制器则支持用户在一组不同的屏幕之间切换，每个屏幕都代表应用程序的一种不同的操作模式。