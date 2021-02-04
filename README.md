 ![LighthouseOS](https://raw.githubusercontent.com/lighthouse-os/manifest/raft/LightHouseBanner.png)

 Getting Started:
 ==============

To get started with manifest/lighthouse, you'll need to get familiar with [Repo](https://source.android.com/source/using-repo.html) and Version Control with [Git](https://source.android.com/source/version-control.html).

To set up build environment:
```
sudo apt update && sudo apt upgrade
git clone https://github.com/akhilnarang/scripts --depth 1
cd scripts
bash setup/android_build_env.sh
```

To initialize your local repository, use a command like this:

```bash
repo init -u git://github.com/lighthouse-os/manifest.git -b raft;

```
You can alternatively use this command to save some space and time :

```bash
repo init --depth=1 -u git://github.com/lighthouse-os/manifest.git -b raft;

```

Then to sync up:

```
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags;
```
You can just use `repo sync` or above command, but this will save you from lot of terminal spam, data and time.
```bash
repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all);
```
---------------------------------------------------------------------------------------
 Compilation of Project Lighthouse:
 ==================

From root directory of project, perform following commands in terminal

```bash
$ . build/envsetup.sh
$ lunch lighthouse_<device_codename>-<build-type>
$ mka lighthouse
```
---------------------------------------------------------------------------------------
 Team Project Lighthouse
 ===============

 * [**Vyom Desai (CannedShroud)**](https://t.me/CannedShroudted) - Core Developer
 * [**Shoury Sharma (galanteria01)**](https://t.me/galanteria01) - Core Developer
 * [**Rishawn Iyer (Stealth1226)**](https://t.me/Stealth1226) - Core Developer

 
---------------------------------------------------------------------------------------
 Credits:
 =======

 * [**AOSP**](https://github.com/AOSP)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**Evolution-X**](https://github.com/Evolution-X)
 * [**CarbonRom**](https://github.com/CarbonRom)
 * [**Pixel Experience**](https://github.com/PixelExperience)
 * [**ManyMore from where cherry-picked from**](https://github.com)

---------------------------------------------------------------------------------------
