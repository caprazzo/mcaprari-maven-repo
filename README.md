Mcaprari maven repository
=========================

## To deploy a release:

    mvn -DaltDeploymentRepository=repo::default::file:../mcaprari-maven-repo/releases/ clean deploy

## To deply a snapshot:

    mvn -DaltDeploymentRepository=snapshot-repo::default::file:../mcaprari-maven-repo/snapshots clean deploy

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



