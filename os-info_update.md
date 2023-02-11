# os-info Update

## Instlal
```
apt install osinfo-db-tools intltool make git
apt install python3-pytest python3-lxml python3-requests gettext
```

## Build

Cloning to osinfo-db
```
git clone https://gitlab.com/libosinfo/osinfo-db
```

```
export SOURCE_DATE_EPOCH="$(date +%s)"
cd osinfo-db
make
```

## Install

```
mkdir builder
osinfo-db-import --root ~/builder/ --system osinfo-db/osinfo-db-YYYYMMDD.tar.xz
cp -Rv * /
```

