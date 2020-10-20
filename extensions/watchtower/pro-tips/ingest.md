# Ingest and proxy workflow

Premiere Pro allows you to ingest media in the background while you are editing.  
You can choose one of four following operations to begin automatically when files are imported into the project:

* **Copy**
* **Transcode**
* **Create Proxies**
* **Copy and Create Proxies**

Due to [Watchtower logic](../how-it-works.md) only **Create Proxies** option is supported by Watchtower.  
Copy/Transcode will change original path of imported media file to a new path and Watchtower will import original file again, creating an infinite loop.

Workarounds for other options are listed below.

## Workarounds

{% tabs %}
{% tab title="Copy" %}
1. Open Ingest Settings. `mac: File > Project Settings > Ingest Settings win: Edit > Project Settings > Ingest Settings`
2. Turn ingest off.
3. Create destination folder you want your media be copied to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually copy files needed to destination folder.
6. With autosync on, files will be automatically imported to the project. Otherwise click force sync button on Watchtower panel to import all new files
{% endtab %}

{% tab title="Transcode" %}
1. Open Ingest Settings. `mac: File > Project Settings > Ingest Settings win: Edit > Project Settings > Ingest Settings`
2. Turn ingest off.
3. Create destination folder you want your media be transcoded to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually add files to Media Encoder and set export settings.
6. Set output to destination folder and start render.
7. With autosync on, files will be automatically imported to the project. Otherwise click force sync button on Watchtower panel to import all new files

{% hint style="info" %}
If you have new files coming from e.g. another editor and would like them to be transcoded and auto imported in the project, you can set up watch folder in Media Encoder, which will output to Watchtower watch folder.⚔Double watch folder ⚔ 
{% endhint %}
{% endtab %}

{% tab title="Copy and Create Proxies" %}
1. Open Ingest Settings. `mac: File > Project Settings > Ingest Settings win: Edit > Project Settings > Ingest Settings`
2. Turn ingest on and set it to Create Proxies.
3. Create destination folder you want your media be copied to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually copy files needed to destination folder.
6. With autosync on, files will be automatically imported to the project. Otherwise click force sync button on Watchtower panel to import all new files.
7. Proxies will be automatically created and attached to imported media.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
To learn more about Ingest and Proxy workflow visit [Premiere Pro User Guide](https://helpx.adobe.com/premiere-pro/using/ingest-proxy-workflow.html).
{% endhint %}

