To upload a release to Maven Central you first must follow the [OSSRH guide](http://central.sonatype.org/pages/ossrh-guide.html) to register an account and receive permissions to the org.mini2Dx project group.

Once you've registered, set up your PGP key per the guide [here](http://nemerosa.ghost.io/2015/07/01/publishing-to-the-maven-central-using-gradle/) and add the required details to ~/.gradle/gradle.properties.

Then you can build and publish a release with the following command:
```bash
./gradlew -Prelease clean build uploadArchives closeAndReleaseRepository
```
