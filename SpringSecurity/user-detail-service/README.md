# Spring Security的UserDetailsService接口

要使用自定以的UserDetailsService只需要关注这几点：

1. UserDetail是spring security中代表了用户数据的顶级接口，可以自己实现该接口，
然后即可在UserDetailsService的loadByUsername中返回，并在程序中各处访问。

2. UserDetailsService是spring security获取用户数据的顶级接口，只要简单的在实现类上配上注解@Configuration即可使用，
spring security是通过的UserDetailsService的实现类来获得用户的信息，进而进行认证。
