**README**

1. Compile the project
2. copy the following files to the output directory:
    - instru.mf
    - application.mf
    - bytebuddy-1.10.22.jar
3. from the output directory, execute the following commands:
   *  jar cfm instrumentation.jar .\application.mf .\Main.class
   * jar cfm simpleInstrumentation.jar instru.mf .\SimpleInstru.class '.\SimpleInstru$TimeFooter.class'
   * java -javaagent:simpleinstrumentation.jar -jar instrumentation.jar
