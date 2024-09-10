# Pro Tips

## Update image sequences

By default Premiere Pro doesn't update image sequences, like After Effect does. Whenever new files are added to image sequence, you will need to offline media and relink it to image sequence again.

With Watchtower image sequences will be updated, turn auto sync on and it will happen in background.

***

## Watchtower + Post Haste

[Post Haste](https://www.digitalrebellion.com/posthaste/) is a free project management tool that allows you to setup file and folder templates for your projects.

When using Watchtower with Post Haste you will be able to setup a project template that will have auto sync feature without need to open Watchtower panel.

### Setting up template project

{% tabs %}
{% tab title="Text only" %}


1. Open Post Haste and navigate to your template.
2. Right click on template top folder and select "Reveal in Finder/Explorer".
3. Copy "Files" folder with template folder structure and paste it to temporary location (e.g. "Desktop").
4. Open template project you just pasted (e.g. "Desktop" location) and then Watchtower Select Folders.\
   In Standard select folders from template folder structure.
5. In Advanced set all folders to **relative path** ("R" checkbox). Adjust other settings if needed.
6. Selected folders will be added to project.
7. Save modified template project and copy it.
8. Replace original template project with modified one.
{% endtab %}

{% tab title="Text with Images" %}


* Open Post Haste and navigate to your template

<div align="center">

<img src="../../.gitbook/assets/post_haste_01.png" alt="">

</div>

* Right click on template top folder and select "Reveal in Finder/Explorer"

![](../../.gitbook/assets/post\_haste\_02.png)

* Copy "Files" folder with template folder structure and paste it to temporary location (e.g. "Desktop").

![](../../.gitbook/assets/post\_haste\_03.png)

* Open template project you just pasted (e.g. "Desktop" location) and then Watchtower Select Folders.\
  In Standard select folders from template folder structure..

![](../../.gitbook/assets/post\_haste\_04.png)

* In Advanced set all folders to **relative path** ("R" checkbox). Adjust other settings if needed.

![](../../.gitbook/assets/post\_haste\_05.png)

* Selected folders will be added to project.

![](../../.gitbook/assets/post\_haste\_06a.png)

* Save modified template project and copy it.

![](../../.gitbook/assets/post\_haste\_07.png)

* Replace original template project with modified one.

![](../../.gitbook/assets/post\_haste\_08.png)
{% endtab %}
{% endtabs %}

{% hint style="info" %}
After setting up template project Watchtower panel could be closed, auto sync will work in background
{% endhint %}

{% hint style="info" %}
If you want to sync folder out of template folder structure use absolute path. (e.g. "Music Libary", "Downloads")
{% endhint %}

***

## Ingest and proxy workflow

Premiere Pro allows you to ingest media in the background while you are editing.\
You can choose one of four following operations to begin automatically when files are imported into the project:

* **Copy**
* **Transcode**
* **Create Proxies**
* **Copy and Create Proxies**

Due to [Watchtower logic](how-it-works.md) only **Create Proxies** option is supported by Watchtower.\
Copy/Transcode will change original path of imported media file to a new path and Watchtower will import original file again, creating an infinite loop.

Workarounds for other options are listed below.

### Workarounds

{% tabs %}
{% tab title="Copy" %}
1.  Open Ingest Settings.

    `mac: File > Project Settings > Ingest Settings`

    `win: Edit > Project Settings > Ingest Settings`
2. Turn ingest off.
3. Create destination folder you want your media be copied to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually copy files needed to destination folder.
6. With autosync on, files will be automatically imported to the project.\
   Otherwise click force sync button on Watchtower panel to import all new files
{% endtab %}

{% tab title="Transcode" %}
1.  Open Ingest Settings.\
    `mac: File > Project Settings > Ingest Settings`

    `win: Edit > Project Settings > Ingest Settings`
2. Turn ingest off.
3. Create destination folder you want your media be transcoded to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually add files to Media Encoder and set export settings.
6. Set output to destination folder and start render.
7. With autosync on, files will be automatically imported to the project.\
   Otherwise click force sync button on Watchtower panel to import all new files

{% hint style="info" %}
If you have new files coming from e.g. another editor and would like them to be transcoded and auto imported in the project, you can set up watch folder in Media Encoder, which will output to Watchtower watch folder.:crossed\_swords:Double watch folder :crossed\_swords:&#x20;
{% endhint %}
{% endtab %}

{% tab title="Copy and Create Proxies" %}
1.  Open Ingest Settings.\
    `mac: File > Project Settings > Ingest Settings`

    `win: Edit > Project Settings > Ingest Settings`
2. Turn ingest on and set it to Create Proxies.
3. Create destination folder you want your media be copied to.
4. Add this folder using Watchtower. A bin will be created in the project.
5. Manually copy files needed to destination folder.
6. With autosync on, files will be automatically imported to the project.\
   Otherwise click force sync button on Watchtower panel to import all new files.
7. Proxies will be automatically created and attached to imported media.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
To learn more about Ingest and Proxy workflow visit [Premiere Pro User Guide](https://helpx.adobe.com/premiere-pro/using/ingest-proxy-workflow.html).
{% endhint %}

