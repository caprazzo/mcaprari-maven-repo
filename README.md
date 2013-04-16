Mcaprari maven repository
=========================

## To deploy a release:

    mvn -DaltDeploymentRepository=repo::default::file:../mcaprari-maven-repo/releases/ clean deploy

## To deply a snapshot:

    mvn -DaltDeploymentRepository=snapshot-repo::default::file:../mcaprari-maven-repo/snapshots clean deploy

## Using this repo in a project:

	<repositories>
	    <repository>
	        <id>mcaprari-releases</id>
	        <url>https://github.com/mcaprari/mcaprari-maven-repo/raw/master/releases</url>
	    </repository>
	    <repository>
	        <id>mcaprari-snapshots</id>
	        <url>https://github.com/mcaprari/mcaprari-maven-repo/raw/master/snapshots</url>
	    </repository>
	</repositories>

## Project pom distribution management

	<distributionManagement>
        <repository>
            <id>repo</id>
            <url>https://github.com/mcaprari/mcaprari-maven-repo/raw/master/releases</url>
        </repository>
        <snapshotRepository>
            <id>snapshot-repo</id>
            <url>https://github.com/mcaprari/mcaprari-maven-repo/raw/master/snapshots</url>
        </snapshotRepository>
    </distributionManagement>    

    



