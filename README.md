# TWRP device tree for Samsung S7 aka herolte

 Copyright (C) 2019 Ananjaser1211 Open-source

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.


Add to `.repo/local_manifests/herolte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="ananjaser1211/android_device_samsung_hero" path="device/samsung/herolte" remote="github" revision="herolte" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_herolte-eng
make -j64 recoveryimage
```

Kernel sources are available at: https://github.com/exynos-linux-stable/herolte
