# Quantaril documentation site

状態: `DOCUSAURUS BUILD READY / NOT DEPLOYED / CONTENT NOT MIGRATED`

QuantarilのP2P／Distributed World Fabricを公開するdocumentation siteです。Target URL: `https://quantaril.i-s.dev/`

横断規約正本は[ZeroRoomLab-manifest](https://github.com/saitoomituru/ZeroRoomLab-manifest)、PLI／CLI envelope正本は[SphereOS-Atlantis](https://github.com/saitoomituru/SphereOS-Atlantis)です。[旧quantaril.cloud](https://github.com/HIPSTAR-IScompany/quantaril.cloud)はlegacy lineageであり、現在仕様へ自動昇格しません。本repositoryはdocs projectionです。

MAGIは公開`main`採用。Docusaurusは実装済み（`npm ci && npm run build`が独立repositoryで再現可能）。Sakura deployは未実装（Q Atlantis #23、CIはbuild jobのみ）、content migrationは未着手（#28）です。code等はApache-2.0、一般文書・図・FlavorはCC BY 4.0を既定候補とします。

## local preview

```console
npm ci
npm start
```

`http://localhost:3000/` でplaceholder siteを確認できます。

## build と検査

```console
npm ci
npm run typecheck
npm run check:domain-hardcode
SITE_ID=quantaril-docs PUBLICATION_URL=https://quantaril.i-s.dev npm run build
SITE_ID=quantaril-docs PUBLICATION_URL=https://quantaril.i-s.dev npm run check:seo
SITE_ID=quantaril-docs npm run receipt:build
```

`SITE_ID` / `PUBLICATION_URL` は`.github/workflows/build.yml`のCI既定値と一致させる。config直書きにせず、常にenv経由で注入する。
