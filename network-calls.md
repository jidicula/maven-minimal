<details><summary>CLI logging</summary>
<p>
[DEBUG] Repositories (dependencies): [github (https://maven.pkg.github.com/jidicula/maven-minimal, default, releases+snapshots), central (https://repo.maven.apache.org/maven2, default, releases)]
[DEBUG] Using transporter HttpTransporter with priority 5.0 for https://maven.pkg.github.com/jidicula/maven-minimal
[DEBUG] Using connector BasicRepositoryConnector with priority 0.0 for https://maven.pkg.github.com/jidicula/maven-minimal with username=jidicula, password=***
Downloading from github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-metadata.xml
[DEBUG] Could not find metadata com.mycompany.app:maven-minimal:1.0-SNAPSHOT/maven-metadata.xml in github (https://maven.pkg.github.com/jidicula/maven-minimal)
Uploading to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.jar
Uploaded to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.jar (2.9 kB at 993 B/s)
Uploading to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.pom
Uploaded to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.pom (2.9 kB at 941 B/s)
Downloading from github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml
Downloaded from github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml (242 B at 461 B/s)
Uploading to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-metadata.xml
Uploaded to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-metadata.xml (774 B at 3.1 kB/s)
Uploading to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml
Uploaded to github: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml (322 B at 1.9 kB/s)
</p>
</details> 

## Steps
1. Attempt download `metadata.xml` for version: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-metadata.xml
   1. Receive 404 because version doesn't exist yet.
2. Upload `.jar`: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.jar
3. Upload `pom.xml`: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-minimal-1.0-20240104.001320-1.pom
4. Download `metadata.xml`: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml
   * note this is the `metadata.xml` for the package.
5. Upload `metadata.xml`: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/1.0-SNAPSHOT/maven-metadata.xml
   * note this is the `metadata.xml` for the package version.
6. Upload `metadata.xml`: https://maven.pkg.github.com/jidicula/maven-minimal/com/mycompany/app/maven-minimal/maven-metadata.xml
   * note this is the `metadata.xml` for the package.
