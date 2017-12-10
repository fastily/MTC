# MTC!
[![Build Status](https://travis-ci.org/fastily/mtc.svg?branch=master)](https://travis-ci.org/fastily/mtc)
![JDK-1.8+](https://upload.wikimedia.org/wikipedia/commons/7/75/Blue_JDK_1.8%2B_Shield_Badge.svg)
[![License: GPL v3](https://upload.wikimedia.org/wikipedia/commons/8/86/GPL_v3_Blue_Badge.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html)

MTC! is a tool that helps simplify and automate the file imports from Wikipedia to Commons.

#### Build
First, clone [jwiki](https://github.com/fastily/jwiki), build, and publish it to your local maven repository:
```bash
git clone --depth 1 https://github.com/fastily/jwiki.git && \
cd jwiki && \
./gradlew -x test build publishToMavenLocal
```

Then, clone and build this project with:
```bash
git clone https://github.com/fastily/mtc.git && \
cd mtc && \
./gradlew build mtc-ui:doDist
```

#### Run
```bash
./gradlew mtc-ui:run
```