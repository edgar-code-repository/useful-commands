UNIX COMMANDS
-----------------------------------------------------------------------

Useful unix scripts.

-----------------------------------------------------------------------

**Executing a java app from a Bash Unix script:**

```

DIR_JAVA_APP=<SOME_PATH>
CLASSPATH_APP=$DIR_JAVA_APP/AppJava.jar

echo "Executing Java app..."

$JAVA_HOME/bin/java -cp $CLASSPATH_APP <fully_qualified_name_of_main_class>
result=$?

echo "Result: $result"

```

-----------------------------------------------------------------------