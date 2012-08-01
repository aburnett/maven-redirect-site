maven-redirect-site
===================

Maven site plugin that generates a simple index page which redirects to another url.

Usage
-----
Create src/site/site.xml


    <project>
        <custom>
            <!-- specify the redirect target here. POM variables can be used. -->
            <redirectTarget>http://somedomain.com/${project.name}</redirectTarget>
        </custom>
        <skin>
	        <groupId>net.thebur</groupId>
            <artifactId>redirect-site</artifactId>
            <version>1.0</version>
        </skin>
    </project>