Spring 4 Framework Code plays uploaded here 
Copyright 2016-17 Syed Awase TPRI/SYCLIQ


=> Regular Expression patterns within the pathvariable 
<bean class="org.springframework.web.servlet.mvc.annotation.RequestMappingHandlerMapping ">
<property name="useRegisteredSuffixPatternMatch" value="false"></property>
</bean>

alternatively use 
@RequestMapping(value="/domain/{domainName:.+}",method=RequestMethod.GET)
public ModelAndView(View domain(@PathVariable("domainName") String domain){
 return new ModelandView("page","page","the domain name is:"+domainName);
}
