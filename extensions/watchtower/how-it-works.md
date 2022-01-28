# How it works

Watchtower uses idea of watch folders — pre-defined folders that constantly look for any new content that is added to them.\
If new content is found, it is automatically added to Premiere Pro/After Effects.

Watchtower compares **file paths** of already imported media and incoming media to determine if file is not in the project and should be imported.

{% hint style="warning" %}
sometimes file could have multiple file paths,\
e.g. mapped drive path vs UNC path on Windows:\
**Z:\Media\file.mov** vs **\\\Server\Media\file.mov**\
****\
****Watchtower considers these files different (same way as Premiere Pro & After Effect does)**.** By default Watchtower will always use UNC path for import.\
If you manually imported file via mapped drive path, Watchtower will import it again, but with UNC path.
{% endhint %}
