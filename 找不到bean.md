***************************
APPLICATION FAILED TO START

***************************

这样的提示是启动类上没有加上@MapperScan(value = "com.leyou.item.mapper")

或者在mapper类上加上@Mapper

Description:

Field categoryMapper in com.leyou.item.service.CategoryService required a bean of type 'com.leyou.item.mapper.CategoryMapper' that could not be found.


Action:

Consider defining a bean of type 'com.leyou.item.mapper.CategoryMapper' in your configuration.

