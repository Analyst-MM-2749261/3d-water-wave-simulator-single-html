# Third-Party Notices

This project distributes a bundled single-file HTML application. The bundled
artifact includes third-party JavaScript libraries and generated CSS. Their
copyright and license notices must be preserved when the application is
redistributed.

## Bundled runtime components

| Component | Bundled version / source identity | License | Notice retained in HTML | Full license file |
|---|---:|---|---|---|
| React | 18.3.1 | MIT | Yes | `third_party/licenses/react-18.3.1-LICENSE.txt` |
| ReactDOM | 18.3.1 | MIT | Yes | `third_party/licenses/react-dom-18.3.1-LICENSE.txt` |
| Modernizr | 3.0.0pre custom build, embedded in ReactDOM bundle | MIT | Yes | `third_party/licenses/modernizr-3.0.0pre-custom-build-NOTICE.txt` |
| three.js | r128 / 0.128.0-equivalent bundled artifact | MIT | Yes | `third_party/licenses/three-r128-LICENSE.txt` |
| D3 | 7.8.5 | ISC | Yes | `third_party/licenses/d3-7.8.5-LICENSE.txt` |
| Tailwind CSS | 3.4.17 generated CSS | MIT | Yes | `third_party/licenses/tailwindcss-3.4.17-LICENSE.txt` |

## Distribution policy

When publishing or redistributing this repository, keep the following together:

1. `index.html`
2. `LICENSE`
3. `THIRD_PARTY_NOTICES.md`
4. `third_party/licenses/`

Do not remove the license header comments embedded in `index.html`. If the
application is re-bundled, regenerate this file and the license inventory from
the actual bundled dependency versions.

## Notes

- The project-level `LICENSE` applies to this repository's original application
  code, documentation, and repository-level assets unless otherwise stated.
- Third-party components remain under their own licenses.
- No Apache-2.0 NOTICE file obligation was identified in the bundled runtime
  components listed above. Re-check this statement if new dependencies are
  added.
