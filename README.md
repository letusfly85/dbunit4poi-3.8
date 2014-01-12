<pre><code>
svn checkout https://svn.code.sf.net/p/dbunit/svn/tags/dbunit-2.4.9 dbunit

(edit your pom.xml)

mvn install:install-file -Dfile=ojdbc14.jar -DgroupId=com.oracle -DartifactId=ojdbc14 -Dversion=10.2.0.4.0 -Dpackaging=jar -DgeneratePom=true

mvn -Dmaven.test.skip=true
</code></pre>
