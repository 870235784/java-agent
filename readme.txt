使用方法：
	1.执行Class文件:
		java -javaagent:%java-agent.jar_path%/java-agent.jar[=args] Class_Name
			%java-agent.jar_path%表示java-agent.jar包的位置
			=args表示传入premain方法的参数
			Class_Name表示运行的Class文件的类名
	2.执行jar包:
		java -javaagent:%java-agent.jar_path%/java-agent.jar[=args] -jar %jar_path%jar_Name
			%jar_path%表示执行的jar包所在的位置
			jar_Name为jar包的名称
	3.tmocat中:
		set JAVA_OPTS=-javaagent:%java-agent.jar_path%/java-agent.jar[=args]