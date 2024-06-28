# subversive
subversive P2 update site

## Mirrored repos
- 4.0/update-site mirrored from https://download.eclipse.org/technology/subversive/4.0/update-site/
- 6.0/update-site mirrored from http://community.polarion.com/projects/subversive/download/eclipse/6.0/update-site/

## Note
There was modification required for the 4.0\update-site\content.jar:
- This contains a reference to the update site http://download.eclipse.org/tools/gef/updates/releases<br>
  This will break Oomph installations of former Eclipse platform versions, running with JVM 1.8 runtime
  since it now enforces installation of Eclipse >=2022-03 artifacts that require a >=Java 11 runtime
  leading to other issues with Java 8 based dev environments.

## Update Site
This repos [p2site](../../tree/main/p2site) content is provided via update site https://p2site.github.io/p2.subversive
