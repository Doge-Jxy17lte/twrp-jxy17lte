## TWRP device tree for Samsung Galaxy J5 2017 (J5Y17LTE)

 Copyright (C) 2018 DevKingsTeam Open-source

 Copyright (C) 2019 Griffin

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.


Add to `.repo/local_manifests/j5y17lte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
  <project name="j5y17lte/twrp-jxy17lte" path="device/samsung/j5y17lte" remote="github" revision="j5y17lte" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_j5y17lte-eng
make -j64 recoveryimage
```

Kernel sources are available at: https://github.com/j5y17lte/kernel-exynos7870
