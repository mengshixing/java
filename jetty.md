1 jetty可以添加Filter,在其中可以加入http Header配置
	
  final HttpServletResponse httpResponse = (HttpServletResponse) response;				
  httpResponse.setHeader("Access-Control-Allow-Origin", "http://192.168.0.124:88");
  //httpResponse.addHeader("Access-Control-Allow-Methods", "GET, POST, PUT, DELETE, OPTIONS");
  //httpResponse.setHeader("Access-Control-Allow-Headers", "x-requested-with");
  //httpResponse.addHeader("Access-Control-Max-Age", "1800");//30 min
  
  对于addHeader() 和 setHeader()这两个方法，可能我们在需要的时候，用起来感觉都一样，都能达到想要的效果。但是这两个方法本质上是不一样的。
  setHeader(name, value)：如果Header中没有定义则添加，如果已定义则用新的value覆盖原用value值。
  addHeader(name, value)：如果Header中没有定义则添加，如果已定义则保持原有value不改变。
