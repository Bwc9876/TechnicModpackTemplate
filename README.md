# AutoModpack

A template you can use to create Technic launcher mod packs through GitHub.

## Setting Up Your Modpack

1. Install your mods on your local machine, [this tutorial](https://help.akliz.net/docs/install-forge-mods-on-a-client) has a good explanation.

2. Ensure all your mods are functioning and configure them to your liking.

3. Open `%APPDATA%\.minecraft` (this can be done by pressing Windows key + R and then pasting it in).

4. Copy the contents of the `mods` and `configs` folders and into the `mods` and `configs` folder of the repo respectively.

5. Download [the universal modpack jar](https://files.minecraftforge.net/net/minecraftforge/forge/index_1.12.2.html) for your Minecraft version.

6. If only the installer is available, install forge normally and head to `%APPDATA%/.minecraft/versions`, select your forge version, and copy the jar file there

6. Rename this jar file to `modpack.jar` and place it in the `bin` folder of the repo.

7. Commit And Push.

## Publishing Your Modpack

1. Select the "Actions" tab in GitHub and press "Create Release", then press the "run workflow" button, and confirm.

2. This will automatically create a new GitHub release for your modpack in the form of a zip file, set the version to something like `0.0.1`.

3. After the build finishes, Head back to the "Code" tab and right-click the "Releases" and copy the link, we'll need this later.

4. Head to the [Technic Platform](https://www.technicpack.net/modpack/create) and make a new modpack.

5. Select "Edit Modpack" and paste that url we copied earlier into the "Modpack location field", then add `/latest/download/modpack.zip` to the end of it.

6. Click "Update Modpack" at the bottom

## Installing Your Modpack

1. Open Technic

2. (If your modpack is hidden) Go to the overview page of your modpack on the Technic website, copy the URL, and place it in the search bar.

3. (If your modpack is public) Search for your modpack.

4. Install, Run, and check to make sure everything is working.

## Installing Your Modpack On A Server (Linux)

Requires `wget` and `unzip`.

```bash
wget "https://github.com/{username}/{repo_name}/releases/latest/download/modpack.zip" && unzip modpack.zip
```

## Updating Your Modpack 

1. Edit whatever files on your local machine and commit/push.

2. Go to the "Actions" tab and select "Create Release".

3. Select "run workflow" and make the version number a higher one than last time.

4. Wait for the action to finish

5. Head to Technic, edit the modpack and select "Versions", fill out your new version number and the change notes.
