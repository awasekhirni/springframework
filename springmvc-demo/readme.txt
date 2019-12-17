SPRING MVC FRAMEWORK
Copyright 2014-15 SYCLIQ/TPRI AWASE KHIRNI SYED 


Resolution for QueryStringParameter containing special characters or "."
for example:http://www.hosting.com/domain/www.amazon.com
/domain/{domainName}

=> dispatcher-servlet.xml 
=> add bean 
<bean class="org.spring.web.servlet.mvc.annotation.DefaultAnnotation">
<property name="useDefaultSuffixPattern" value="false"></property>
<bean>

