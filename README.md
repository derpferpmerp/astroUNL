# astroUNL
every swf from astroUNL's project, for astronomy
Built by (zip = astroUNL.zip):
```sh
mkdir astro
cd astro
mv ../astroUNL.zip ./
unzip astroUNL.zip
chmod -R 777 *
mkdir swfs
find ./astroUNL -type f -name '*.swf' -exec mv -i {} ./swfs/ \;
tar -cvf tarred.tar.gz ./swfs
curl -T tarred.tar.gz -Lv station307.com 2>&1 | grep located-at
```
or just git clone my repo

Next, navigate to [ruffle](https://ruffle.rs), or use an emulator,
navigate to demo (or if not on chromebook, download it),
and then upload (if on demo) any swf file to use it, or use the app
if not on chromebook or if on a supported platform.

The release is the full source code of the webpage, so if you want to build it yourself (the first shell script),
you can just download that and use that as the archive to run (make sure to rename it to astroUNL.zip)
