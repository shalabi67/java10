#First
##compile
javac -d out src/com/learn/learn_modules/*.java src/module-info.java

##generate jar file
md lib
jar --create --file lib/first.jar -C out .

##run first application
java  --module-path out --module com.learn.learn_modules/com.learn.learn_modules.Application
###or
java  --module-path lib --module com.learn.learn_modules/com.learn.learn_modules.Application

