# HBase Connectors - TDP

## Build

```
mvn clean install \
  -DskipTests \
  -Dmaven.javdoc.skip=true \
  -Dcheckstyle.skip=true \
  -Dfindbugs.skip=true \
  -Dspotbugs.skip=true \
  --batch-mode \
  -fae
```
## Build with specific dependencies

```
mvn clean install \
  -Dspark.version=2.3.4-1.0 \
  -Dscala.version=2.11.8 \
  -Dscala.binary.version=2.11 \
  -Dhadoop-three.version=3.1.1-0.0 \
  -Dhbase.version=2.1.10-1.0 \
  -DskipTests \
  -Dmaven.javdoc.skip=true \
  -Dcheckstyle.skip=true \
  -Dfindbugs.skip=true \
  -Dspotbugs.skip=true \
  --batch-mode \
  -fae
```

## Test

```
mvn clean test \
  --batch-mode \
  --fail-never
```
