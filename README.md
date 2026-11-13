# Huawei Health Customization v2.0 — International HWT Import

Fork build for **Huawei Health 17.0.8.300 / 17.0.8.320** with additional allowed watchface store hosts:

- `h5hosting-drcn.dbankcdn.cn` (China)
- `h5hosting-dra.dbankcdn.com` (international)
- `h5hosting-dre.dbankcdn.com` (international)

## Reproducible build

The GitHub Actions workflow pins upstream source to commit
`cc9c24eb8dcfcf7050b034f56966d7f32472d487`, applies
`international.patch`, imports the patched full source to this repository,
and builds a **debug-signed APK** as a workflow artifact.

Open **Actions → Build International HWT Import → latest run → Artifacts**.
This is **not a Huawei-official APK**, and installing it cannot guarantee the
HWT import will succeed on a GT 7 Pro, especially on firmware that blocks
third-party watchface installations.

The upstream source is licensed under GPL-3.0. The original LICENSE is
preserved during source import. The international patch permits only three
named HTTPS domains with the exact watchface storefront path.

Do not install an APK if the workflow failed or the artifact is missing.
