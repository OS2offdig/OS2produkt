# Include a Publiccode.yml file in the project

Publiccode.yml is a metadata standard for repositories containing software developed or acquired by the Public Administration, aimed at making them easily discoverabile and thus reusable by other entities.

By including a publiccode.yml file in the root of a repository, and populating it with information about the software, technicians and civil servants can evaluate it. Automatic indexing tools can also be built, since the format is easily readable by both humans and machines.

Full documentation is available [here](https://docs.italia.it/italia/developers-italia/publiccodeyml-en/en/master/index.html).

A guide explaining how to add the publiccode.yml file to your project can be [found here](https://publiccode.discourse.group/t/how-do-i-add-a-publiccode-yml-file-to-my-project/28).


## Example of a minimal version

```
publiccodeYmlVersion: "0.2"

name: Medusa
url: "https://example.com/italia/medusa.git"
softwareVersion: "dev"    # Optional
releaseDate: "2017-04-15"
platforms:
  - web

categories:
  - financial-reporting

developmentStatus: development

softwareType: "standalone/desktop"

description:
  en:
    localisedName: medusa   # Optional
    genericName: Text Editor
    shortDescription: >
          A rather short description which
          is probably useless

    longDescription: >
          Very long description of this software, also split
          on multiple rows. You should note what the software
          is and why one should need it. We can potentially
          have many pages of text here.

    features:
       - Just one feature

legal:
  license: AGPL-3.0-or-later

maintenance:
  type: "community"

  contacts:
    - name: Francesco Rossi

localisation:
  localisationReady: yes
  availableLanguages:
    - en
```
